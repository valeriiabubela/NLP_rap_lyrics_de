<h2>Rap lyrics generation in German with GPT-2</h2> 
<p>This project was done as a part of the seminar "Natural Language Processing" at the Free University of Berlin.
<h3>Dataset</h3> 
<p>For finetuning, a combination of two datasets was used. Originally, I planned to only use <a href="https://huggingface.co/dbmdz/german-gpt2" target="_blank">this German Rap Dataset</a> from Kaggle. It includes 700 files but after deleting empty files und duplicates, only 592 files were left. So I decided to create my own additional dataset using the Python package <a href="https://pypi.org/project/lyricsgenius/" target="_blank">lyricsgenius</a>. This way, 1753 songs from 10 rappers were scraped. In total, the set for finetuning consists of <b>2345 songs</b>. 
<p>→ <kbd>Lyrics_scraping.ipynb</kbd>
<h3>Data cleaning</h3> 
<p>
<p>→ <kbd>Data_cleaning.ipynb</kbd>
<h3>GPT-2 finetuning</h3> 
<p><a href="https://huggingface.co/dbmdz/german-gpt2" target="_blank">German GPT-2 model</a> from Huggingface was finetuned with a combination of datasets mentioned above.
<p>→ <kbd>GPT-2.ipynb</kbd>
<h3>Lyrics generation</h3> 
<p>Lyrics were generated with the help of <a href="https://huggingface.co/transformers/main_classes/pipelines.html#transformers.TextGenerationPipeline" target="_blank">TextGenerationPipeline</a> from Transformers.
<p>→ <kbd>Text_generation.ipynb</kbd>
