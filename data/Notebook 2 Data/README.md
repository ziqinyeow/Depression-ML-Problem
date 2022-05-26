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

## Test Question

Instructions: Beside is a list of questions that relate to life experiences common among people who have been diagnosed with depression. Please read each question carefully, and indicate how often you have experienced the same or similar challenges in the past few months.

1. Little interest or pleasure in doing things
2. Feeling down, depressed, or hopeless
3. Trouble falling or staying asleep, or sleeping too much
4. Feeling tired or having little energy
5. Poor appetite or overeating
6. Feeling bad about yourself - or that you are a failure or have let yourself or your family down
7. Trouble concentrating on things, such as reading the newspaper or watching television
8. Moving or speaking so slowly that other people could have noticed
9. Thoughts that you would be better off dead, or of hurting yourself
10. If you've had any days with issues above, how difficult have these problems made it for you at work, home, school, or with other people?

1 - 9
0 - Not at all.
1 - Several days.
2 - More than half the days.
3 - Nearly every day.

10
0 - Not difficult at all.
1 - Somewhat difficult.
2 - Very difficult.
3 - Extremely difficult.
