# strengthen-scoring

Questionnaire scoring configuration files for the Strengthen project

## How to use this

This is a set of scoresheets (in `scoresheets/`) and a multiscore configuration file (`multiscore.csv`) for use with [scorify](https://github.com/uwmadison-chm/scorify). This program expects one CSV data file per REDCap event, named as `strengthen__{event}.csv` -- so, for example, `strengthen__scr.csv` for the screening event. You'll need one input data file for every unique `short_event` listed in `multiscore.csv`.

Once you have scorify installed, you'd score the dataset with a command similar to:

```
score_multi /path/to/multiscore.csv \
    /path/to/scoresheets/score_{scoresheet}.csv \
    /path/to/redcap_data/strengthen__{redcap_event}.csv \
    /path/to/scored_data/{short_event}_{scoresheet}.csv
```

and that will produce one output file per row in `multiscore.csv`.

See the scorify documentation and `score_multi -h` for more help, email [Nate Vack](mailto:njvack@wisc.edu) , or post to the [scorify discussion groups](https://github.com/uwmadison-chm/scorify/discussions).
```
```
