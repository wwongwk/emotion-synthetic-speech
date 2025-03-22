# Emotion Perception in Synthetic Speech: The Influence of Pitch and Semantics

## About The Project

Emotions in speech are shaped by prosody—such as pitch—and semantic sentiment, which defines the emotional tone of content. This project examines how these factors interact in synthetic speech to influence emotional perception. Using the So-To-Speak interface, we designed a within-subject experiment to isolate pitch effects across positive, neutral, and negative semantics.

## Key Hypotheses

1. Higher pitch conveys happiness, even when semantic content is negative.
2. Lower pitch conveys sadness, irrespective of semantic meaning.
3. High pitch and neutral sentiment convey happiness.
4. Low pitch and neutral sentiment convey sadness.

## Objectives

- Investigate the impact of pitch and semantic sentiment on emotional perception.
- Isolate pitch as a critical factor in shaping emotional judgments in synthetic speech.
- Evaluate whether pitch can override or reinforce semantic meaning.

## Methodology

### Experiment Design

- Within-subjects design with 6 conditions:
  - Combinations of **high/low pitch** and **positive/neutral/negative** semantics.
- Each participant listened to 30 randomized trials (5 per condition).
- Emotional ratings collected on a 7-point Likert scale (1 = Sad, 4 = Neutral, 7 = Happy).

### Speech Samples

Generated using the So-To-Speak interface with controlled pitch levels and semantic content:
- **Positive**: e.g., "She won the lottery yesterday."
- **Neutral**: e.g., "I’ll be here tomorrow."
- **Negative**: e.g., "He lost a huge sum of money."

### Example Audio Files

1. High Pitch + Positive: [Play Audio](https://gabalpha.github.io/read-audio/?p=https://raw.githubusercontent.com/wwongwk/emotion-synthetic-speech/main/audio/P5_high_4.1.wav)  
2. Low Pitch + Positive: [Play Audio](https://gabalpha.github.io/read-audio/?p=https://raw.githubusercontent.com/wwongwk/emotion-synthetic-speech/main/audio/P5_low_3.9.wav)  
3. High Pitch + Neutral: [Play Audio](https://gabalpha.github.io/read-audio/?p=https://raw.githubusercontent.com/wwongwk/emotion-synthetic-speech/main/audio/NT1_high_3.7.wav)  
4. Low Pitch + Neutral: [Play Audio](https://gabalpha.github.io/read-audio/?p=https://raw.githubusercontent.com/wwongwk/emotion-synthetic-speech/main/audio/NT1_low_4.1.wav)  
5. High Pitch + Negative: [Play Audio](https://gabalpha.github.io/read-audio/?p=https://raw.githubusercontent.com/wwongwk/emotion-synthetic-speech/main/audio/NG5_high_3.6.wav)  
6. Low Pitch + Negative: [Play Audio](https://gabalpha.github.io/read-audio/?p=https://raw.githubusercontent.com/wwongwk/emotion-synthetic-speech/main/audio/NG5_low_4.1.wav)  

### Participants

- 29 participants completed the study.

### Analysis

- Data analyzed using a **Linear Mixed Model**.
- Fixed effects: pitch, sentiment, and their interaction.
- Post-hoc comparisons via Tukey’s HSD.

## Results

- **Low pitch significantly decreased emotion ratings** in both positive and neutral contexts, aligning with sadness perception.
- **High pitch did not significantly increase ratings** in neutral or negative contexts.
- Baseline conditions confirmed expectations:
  - High pitch + positive sentiment = significantly higher happiness ratings.
  - Low pitch + negative sentiment = significantly lower sadness ratings.

### Summary Table

| Condition                       | Mean Rating | Significance (vs Neutrality) |
|--------------------------------|-------------|-------------------------------|
| High pitch + Negative (H1)     | 3.98        | Not Significant               |
| Low pitch + Positive (H2)      | 3.17        | **Significant** (p < 0.001)   |
| High pitch + Neutral (H3)      | 4.02        | Not Significant               |
| Low pitch + Neutral (H4)       | 3.54        | **Significant** (p < 0.001)   |
| High pitch + Positive (B1)     | 4.96        | **Significant** (p < 0.001)   |
| Low pitch + Negative (B2)      | 2.70        | **Significant** (p < 0.001)   |

## Conclusion

### Key Findings

- **Low pitch dominates over semantic content**, consistently leading to sadness perception—even with positive or neutral semantics.
- **High pitch only conveyed happiness when paired with positive semantics**, suggesting pitch alone cannot override negative or neutral sentiment.
- The asymmetry reveals that **sadness cues are more robust** and consistent across pitch-semantics interactions, while happiness cues may require more nuanced features like intonation or emotional variation.

### Limitations

- Synthetic speech lacks the full richness of natural vocal expression (e.g., intonation, rhythm).
- Only two emotional categories (happiness, sadness) were studied.
- Results may not generalize to human speech perception.

### Future Work

- Expand emotional range (e.g., anger, fear, surprise).
- Explore additional vocal parameters like **intonation, speech rate, and pauses**.
- Compare synthetic vs. human speech emotion perception.
- Integrate **Russell’s Circumplex Model of Affect** to better capture emotional nuance.

## Contributors

- Yogie Permana  
- Oskar Lövgren  
- Pin-Ju Huang  
- Wei Kang Wong  
- Sabika Amalina

## Acknowledgments

Special thanks to the developers of the **So-To-Speak** interface for enabling this research on controllable synthetic speech and prosody.
