# Phone Number Entity Dataset
Dataset Release for Phone Number Entity capture task

## About

There are two tracks here, and together they explore the task of capturing phone numbers from human speech. As per our knowledge this is the first public dataset for capturing numeric-sequence entities from speech. Each track consists of 2 (Indian English) speakers speaking out 75 phone numbers each:
1. one track has phone numbers spoken in a single utterance, and
2. the other track has phone numbers split across two utterances with a (4,6) split of digits

The audios were recorded over a telephony line.

## Download and Usage

The tracks can be downloaded by clicking on these links:
- [single-turn.zip](https://phone-number-entity-dataset.s3.ap-south-1.amazonaws.com/single-turn-dataset.zip)
- [two-turns.zip](https://phone-number-entity-dataset.s3.ap-south-1.amazonaws.com/two-turn-dataset.zip)

Incase you face any issues, please reach out to kmanas@skit.ai.

This dataset is shared under [Creative Commons Attribution-NonCommercial 4.0 International Licence](https://creativecommons.org/licenses/by-nc/4.0/). This places restrictions on commercial use of this dataset.

## Uses

A phone-number sequence is what we call a *complex* entity, and human speech tends to express such entities in different ways. These range from small pauses within the utterance, to breaking the entity into smaller, simpler pieces. If such patterns are a naturalistic way of speaking, then shouldn't Spoken Dialog Systems model this into their workings ? This dataset is a step towards exploring what such systems look like, and evaluating how they would do in the real-world.

A simple experiment with existing ASR systems would be to evaluate them on each track. The emphasis here is not on competitive performance between systems, but on each system across the tracks - how much better is the entity-capture task, when we model patterns in human speech ?

## Structure

This release contains data of two speakers speaking out 75 phone numbers each in an Indian English accent.

Frequency : 8 Khz

Structure

```

 - single_turn_dataset
   - data                  [contains the wav files]
   - single_turn_data.csv. [contains the entity tag for an audio, where each row contains "<call-id> | <turn-id> | <relative-path> | <tag> | <speaker-id>"]
 - two_turn_dataset
   - data
   - two_turn_data.csv
   
```

More information regarding the dataset can be found in the [datasheet](./datasheet.md).

## Citation

If you are using this dataset, please cite using the link in the About section on the right.

## License

Shield: [![CC BY-NC 4.0][cc-by-nc-shield]][cc-by-nc]

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc].

[![CC BY-NC 4.0][cc-by-nc-image]][cc-by-nc]

[cc-by-nc]: http://creativecommons.org/licenses/by-nc/4.0/
[cc-by-nc-image]: https://licensebuttons.net/l/by-nc/4.0/88x31.png
[cc-by-nc-shield]: https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg
