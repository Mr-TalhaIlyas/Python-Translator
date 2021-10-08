# Python-Translator

For translating the text (e.g., filenames, descriptions etc.) using python scripts.
```
pip install google_trans_new==1.1.9
```

Then open the `google_trans_new/google_trans_new.py` file and cange line `151` in that file from


```response = (decoded_line + ']')```

to 

```response = decoded_line```


Now you can use it as follows,

```python
from google_trans_new import google_translator  
translator = google_translator()  
translate_text = translator.translate('G:/Data/southern_crabgrass/images/바랭이-dat15(45도-1).JPG', # filename expmple
                                       lang_src='kr', # source language kr=> korean
                                       lang_tgt='en') # destination language en=> english
print(translate_text)
```
**Output**

```
G: / DATA / SOUTHERN_CRABGRASS / Images / Barnes -DAT15 (45 degrees -1) .jpg 
```
