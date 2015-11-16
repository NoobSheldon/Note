# GFM=Github Flavored Markdown
## Differences from traditional Markdown
### Multiple underscores in words
def get_attr(): 
### URL autolinking
http://example.com
### Strikethrough
~~Mistaken text.~~
### Fenced code blocks

```
import os,flask
print 'i am good'
```
*indent non-fenced code blocks 8 spaces to render them properly,within lists*
### Syntax highlighting

```python
def json_to_dict(x):
    '''OAuthResponse class can't not parse the JSON data with content-type
    text/html, so we need reload the JSON data manually'''
    if x.find('callback') > -1:
        pos_lb = x.find('{')
        pos_rb = x.find('}')
        x = x[pos_lb:pos_rb + 1]
    try:
        return json.loads(x, encoding='utf-8')
    except:
        return x
```
### Tables
| First Header | second Header |
| ------------ | ------------- |
| Content Cell | Content       |
* *the dashes at the top don't need to match the length of the header text*
* *include inline Markdown such as links,bold,italics,strikethrough*
* *including colons : within the header row,define text to be left-aligned*

### HTML
---------------------------------------
# Other additional features
### Newlines
### Task lists
**Lists can be turned into task lists by prefacing list items with [] or [x]**
**(incomplete and complete,respectively)**   
*Task lists can be nested to better structure your tasks*
### References
# Features
+ Quick quoting
+ Name and team @mentions autocomplete
+ Emoji autocomplete
+ Issue autocomplete
