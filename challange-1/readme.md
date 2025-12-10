# 🚀 Taxi Hotspot Hunt – Uncover the Lost Pulse of Our Startup

Since the early days of creating Yassir, they began noticing something unusual hidden inside the taxi trip data. While the routes looked completely normal on the surface, a strange pattern kept reappearing — almost like a secret hotspot quietly pulsing behind the scenes.

To keep this discovery protected, the dataset was intentionally recorded with subtle distortions:
some trips are incomplete, some clusters are decoys, and even the fares aren’t the real ones. An early developer shifted them using a specific key… and only someone who reads the challenge carefully will figure out how to reverse it


]

## 📂 Your Mission

You have received a file: `taxi_hotspot_dataset.csv`. Each row represents a taxi trip.

Hidden within this dataset are clusters — sequences of 3 trips at the same location that follow a special fare pattern.

A cluster is considered valid if all of the following hold:

### 1️⃣ Different taxis
All 3 trips must have distinct car IDs.

### 2️⃣ Fare pattern
The middle trip's fare B follows this formula:

```
B = |A - C| + (A mod C)
```

Where:
- A = first trip fare
- B = second (middle) trip fare
- C = third trip fare

### 3️⃣ Chronological order
Trips at that location must occur in order by timestamp.

### 4️⃣ Overlapping clusters
Trips can appear in overlapping clusters. Some clusters are decoys: they may look correct but fail one or more rules. Only the correct clusters reveal the hidden hotspot, emerging with the highest combined score.

## 💎 Scoring

- Each valid cluster carries a signature, calculated as the **sum of its fares**.
- The **total score per coordinate** is the sum of all valid cluster signatures at that location.
- More valid clusters → higher total score.
- Decoys and inconsistent trips exist to mislead you.

## ⚖️ Tie-Breaking

If multiple coordinates share the highest score:

1. Pick the coordinate whose **earliest valid cluster** occurs first.
2. If still tied, pick the **largest latitude**.
3. If still tied, pick the **largest longitude**.

## 🕵️‍♂️ Your Tasks

1. Detect all valid clusters following the rules above.
2. Compute total scores per coordinate.
3. Apply tie-breaking rules to determine the true hotspot.

## 📌 Deliverables

1. **(latitude, longitude)** of the hotspot
2. **Name of the place** (verify it's a real location)
3. **Your code** (implementation used to solve the challenge)

## ⚠️ Important Note

The hotspot coordinates must correspond to a **real place**. Verify the latitude and longitude using a mapping service to ensure the location exists and is valid.