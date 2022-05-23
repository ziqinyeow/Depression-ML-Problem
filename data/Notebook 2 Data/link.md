# Data Download

```python
import requests

csv_url_1 = "https://raw.githubusercontent.com/patilgirish815/Depression_Detection_Using_Machine_Learning/main/dataset/depressionDataset.csv"
csv_url_2 = "https://raw.githubusercontent.com/patilgirish815/Depression_Detection_Using_Machine_Learning/main/dataset/tweets.csv"

req = requests.get(csv_url_1)
url_content = req.content
csv_file = open('data.csv', 'wb')
csv_file.write(url_content)

req = requests.get(csv_url_2)
url_content = req.content
csv_file = open('tweet.csv', 'wb')
csv_file.write(url_content)

csv_file.close()
```
