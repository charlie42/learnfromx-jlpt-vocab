# JLPT Vocabulary List, N5 to N1

A free list of 18,136 Japanese words sorted into JLPT levels N5 to N1, as CSV, JSON or a Yomitan dictionary. This is a cleaned-up version of a list we built internally for LearnFromX (https://learnfromx.com) to estimate a learner's level.

The JLPT stopped publishing word lists in 2010. Jisho.org's JLPT tags come from the lists Jonathan Waller compiled around that time. On Jisho, everyday words such as 顔 (face), 母 (mother) and ない (there isn't) have no JLPT level. We kept Waller's lists as the base and added 10,532 words.

Web page: https://learnfromx.com/jlpt-vocabulary-list

## Download

| File | What's in it |
|---|---|
| `jlpt-style-vocab.csv` | Full list |
| `jlpt-style-vocab.json` | Full list, same data as a list of objects |
| `by-level/n5.csv` ... `by-level/n1.csv` | One file per level |
| `learnfromx-jlpt-vocab.zip` | Yomitan dictionary, from the latest release: https://github.com/charlie42/learnfromx-jlpt-vocab/releases/latest |

The CSV files are UTF-8 and open in Excel, Google Sheets and Numbers. Anki can import them too (File, then Import).

## File format

One row per word. The JSON file holds the same data as a list of objects.

| Column | Contents |
|---|---|
| `level` | JLPT level, N5 to N1 |
| `kanji` | How the word is written. Words usually written in kana have kana here, with any kanji spelling after it. |
| `reading` | Reading in kana |
| `meaning` | Short English meaning |
| `in_waller` | `yes` if the word is in Waller's lists, `no` if we added it |
| `waller_level` | Waller's level for the word, blank if he doesn't list it |

Where a word has more than one spelling or reading, the CSV separates them with a semicolon. In the JSON they are arrays. Rows are sorted by level, then from most to least common.

### Words per level

| Level | Words | From Waller | Added |
|---|---|---|---|
| N5 | 1,091 | 914 | 177 |
| N4 | 1,489 | 916 | 573 |
| N3 | 5,561 | 2,517 | 3,044 |
| N2 | 6,684 | 1,501 | 5,183 |
| N1 | 3,311 | 1,756 | 1,555 |
| Total | 18,136 | 7,604 | 10,532 |

Of the 7,604 words from Waller's lists, 5,101 keep his level and we moved 2,503 to a different one. Both levels are in the file.

## Yomitan dictionary

Yomitan is a free pop-up dictionary for Chrome, Firefox and Edge. This dictionary adds a JLPT level tag to each word you look up. It has no meanings of its own, so Yomitan shows the tag next to the entry from your usual dictionary.

1. Download `learnfromx-jlpt-vocab.zip` from the latest release.
2. In Yomitan, open Settings, then Dictionaries, then Import, and choose the zip file.
3. Switch the new dictionary on in the same list.

When we publish a new version, you can get it with the "Check for updates" button on Yomitan's Dictionaries page.

## How the list was made

1. We started from Jonathan Waller's N5 to N1 lists.
2. We added words that come up often in anime dialogue and everyday speech. Each was assigned a level using a large language model.
3. We removed grammar patterns, "can do" verb forms (such as 言える, can say), slang spellings, sound words and names, and merged words that were listed twice, once in kana and once in kanji.

Found a mistake? Please open an issue.

## Frequently asked questions

### Is this the official JLPT vocabulary list?

No. The JLPT has not published an official word list since 2010, so every JLPT vocabulary list, this one included, is an estimate.

### How many words are there at each level?

N5 has 1,091 words. Up to N4 there are 2,580, up to N3 8,141, up to N2 14,825 and up to N1 18,136.

### Can I import the list into Anki?

Yes. In Anki, choose File, then Import, and pick one of the CSV files. With the per-level files, you can make one deck per level.

### How is it different from Waller's lists?

It has every word from Waller's lists plus 10,532 more, mostly common words from everyday speech. Of Waller's words, 2,503 have a different level here. The files show both levels.

## License and attribution

The list is free under CC BY-SA 4.0 (see `LICENSE`), including for commercial use. Please credit it as below and share any changes under the same license.

```
JLPT Vocabulary List by LearnFromX (https://learnfromx.com/jlpt-vocabulary-list), CC BY-SA 4.0. Based on Jonathan Waller's JLPT lists (tanos.co.uk) and JMdict (EDRDG).
```

It is based on Jonathan Waller's JLPT Resources at https://www.tanos.co.uk/jlpt/ (CC BY) and on JMdict by the Electronic Dictionary Research and Development Group, https://www.edrdg.org/ (CC BY-SA 4.0). Some meanings come from JMdict.

Made by LearnFromX (https://learnfromx.com), where you learn Japanese from anime.
