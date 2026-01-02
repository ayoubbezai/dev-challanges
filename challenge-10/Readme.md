# 🧪 Chemical Sequence Decoder

## Challenge Information

**Author:** ayoubbezai  
**Category:** Problem Solving  
**Difficulty:** Medium  
**Type:** Logic Challenge  
**Points:** 400

## 🧠 Description

A chemical researcher and developer has generated a dataset of input → output pairs.

**Key facts:**
- The dataset is fully deterministic
- There are no bugs
- There is no randomness
- Your function must work for ANY input, not just the ones in the dataset

## 🎯 Your Mission

1. Analyze the input-output pairs in `dataset.csv`
2. Discover the hidden pattern(s)
3. Write a function `f(input)` that works for ANY valid input

**Important:** Your function must be generalizable and work correctly even for inputs NOT in the original dataset.

## 🕵️‍♂️ Scoring

* Points: 400
* Your solution must handle all cases correctly
* Function must work for inputs beyond the dataset

## 📌 Deliverables

1. **Function implementation** in any programming language
2. **Documentation** explaining:
   - The pattern you discovered
   - How your function works
   - Why it works for ANY input
3. **Code repository** (GitHub link preferred)

## 💻 Function Template
```python
def f(input):
    """
    Takes an input and returns the corresponding output.
    Must work for ANY valid input, not just dataset examples.
    """
    # Your implementation here
    pass
```

## ⚠️ Important Notes

- The dataset is provided in `dataset.csv` in this repository
- The function must be generalizable
- Brute-force memorization will NOT work
- Your logic must explain ALL cases
- Test with numbers outside the dataset

## 📝 Submission Format
```
chemical-decoder/
├── src/
│   └── decoder.py (or your language)
├── explanation.md
├── README.md
└── requirements.txt (if applicable)
```

Good luck! 🔬