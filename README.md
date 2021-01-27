# kk-wrangle

- Source repo : https://github.com/Krishna-Koyyalamudi/kk-wrangle/

### Assigned Play - 9. Timon of Athens

- Article Source : http://shakespeare.mit.edu/timon/full.html
- Speaker 1 : TIMON
- Speaker 2 : FLAVIUS

### Question Asked

What is the number of times the speaker 1 has dialogue and speaker 2 has dialogue. Also determine the total count of both the dialogues

### Bash commands used :

```Bash
timon=$(grep -i '^TIMON' ToA_data.txt -c)
echo "The count of TIMON dialogues is: ${timon}" > speaker1_count.txt
flavius=$(grep -i '^FLAVIUS' ToA_data.txt -c)
echo "The count of FLAVIUS dialogues is: ${flavius}" > speaker2_count.txt
total=$(( $timon + $flavius ))
echo "The total TIMON & FLAVIUS dialogues is: ${total}" > total_count.txt
```
### Answer:

- TIMON Count - 217
- Flavius Count - 42
- Total Count - 259
