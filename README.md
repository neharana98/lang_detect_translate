# lang_detect_translate
**Overview**:
With the rise of digital communication, a growing number of users are expressing themselves in Hindi (and other Indian languages), using the Roman script. This hybrid form of language, referred to as “Hinglish”, blends Hindi and English — phonetically written using the Roman script, with no standard spellings! While users prefer Hinglish for its ease, it presents a challenge for analysts, especially in language detection and translation.

**Objective**:
To identify which Python library performs the best in detecting and translating Hinglish text.

**Methodology**:
Language detection with open-source libraries:
1. langid
2. langdetect
3. pcyld2
4. fasttext
5. googletrans

Language translation with googletrans

**Findings**:
Googletrans outperformed all other libraries in language detection, showcasing 100% accuracy on our mixed dataset with English and Hinglish text. Traditional libraries like langid, langdetect, and pcyld2 struggled due to their rule-based or keyword-matching systems, often misclassifying languages. Googletrans’s superior performance stems from its Neural Machine Translation (NMT) model, which handles noisy, phonetically inconsistent Hinglish more effectively. However, while detection was strong, translation accuracy stood at 80%, with occasional misinterpretation of idioms, slang, and sarcasm — highlighting the need for more context-aware, Indic-trained models.
