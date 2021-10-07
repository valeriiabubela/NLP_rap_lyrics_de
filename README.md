<h2>Rap lyrics generation in German with GPT-2</h2> 
<blockquote>
Zuhause und Heimat<br>
Ich komme von der Wiege der Stadt<br>
und bleib nie sitzen<br>
Ich komme zu keiner Zeit wenn ich keine Antwort heebe<br>
doch bin doch kein Freund von mir<br>
weil ich schon zu oft im<br>
© GPT-2
</blockquote>
<blockquote>
Kapitalismus ist der Teufel der am Block in dem Auto sitzt<br>
du machst auf die Welt auf<br>
Mach weiter den Weg nach dem ich es mir verdient hab<br>
Alles für die Straße oder für die Heimat<br>
Alles was du willst kannst<br>
© GPT-2
</blockquote>
<p>This project was done as a part of the seminar "Natural Language Processing" at the Free University of Berlin.
<h3>Dataset</h3> 
<p>For finetuning, the following <a href="https://huggingface.co/dbmdz/german-gpt2" target="_blank">German Rap Dataset</a> from Kaggle was used. It includes 700 files but after deleting empty files und duplicates, only <b>592</b> files were left.
<h3>Data cleaning</h3> 
<p>The dataset was cleaned from special characters, letter case was normalised according to a part of speech. Two training corpora were created. For the first one, the dataset was split into songs (<kbd><a href="https://github.com/valeriiabubela/NLP_rap_lyrics_de/blob/main/all_texts_cleaned.json" target="_blank">all_texts_cleaned.json</a></kbd>); for the second one - info refrains (<kbd><a href="https://github.com/valeriiabubela/NLP_rap_lyrics_de/blob/main/refrains.json" target="_blank">refrains.json</a></kbd>).
<p><b>Disclaimer</b>:
<p>→ <kbd><a href="https://github.com/valeriiabubela/NLP_rap_lyrics_de/blob/main/data_cleaning.ipynb" target="_blank">data_cleaning.ipynb</a></kbd>
<h3>GPT-2 finetuning</h3> 
<p><a href="https://huggingface.co/dbmdz/german-gpt2" target="_blank">German GPT-2 model</a> from Huggingface was finetuned with a dataset mentioned above.
<p>→ <kbd><a href="https://github.com/valeriiabubela/NLP_rap_lyrics_de/blob/main/model_finetuning.ipynb" target="_blank">model_finetuning.ipynb</a></kbd>
<h3>Lyrics generation</h3> 
<p>Lyrics were generated with the help of <a href="https://huggingface.co/transformers/main_classes/pipelines.html#transformers.TextGenerationPipeline" target="_blank">TextGenerationPipeline</a> from Transformers.
<p>→ <kbd><a href="https://github.com/valeriiabubela/NLP_rap_lyrics_de/blob/main/text_generation.ipynb" target="_blank">text_generation.ipynb</a></kbd>
<h3>Reflections on the project</h3> 
