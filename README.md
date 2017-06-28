# parse_QIAxcel_csv.py (python2.7)<br />
Generates a user-friendly, tab-separated file from the .csv file(s) generated by the QIAxcel ScreeenGel software (maps sample name, reports dilution factor, selects fragment size).<br />

## Usage<br />

`python parseQIAxcel.py	[-h] [-fol [FOL]] [-out [OUT]] -dil [DIL] -siz [SIZ [SIZ ...]] [-ali ALI ALI] [-sam [SAM [SAM ...]]] [--det] [--plate]<br />`

## Optional arguments:<br />

	`-h`, `--help`            Show help message and exit<br />
	`-fol` [FOLDER]         Folder to start parsing .csv files (default: current folder from where the command line in written)<br />
	`-out` [OUTPUT]         Output file name (default: starting folder name with time stamp and _qiaxcelOut.xls)<br />
	`-dil` [DILUTION]       Dilution factor (needed: one number)<br />
	`-siz` [MIN [MAX]]      Fragment size range (required: min (optional: and max))<br />
	`-ali` MIN MAX          Alignment markers sizes (default = 15 1000)<br />
	`-sam` [FIL1 [FIL2...]] File(s) for sample name mapping. A least three columns are needed: (1) plate name as before ".csv", (2) well coordinates(e.g. A5), (3+) sample name (could be composite but space-separated: e.g. "sample1 DNA 20mg positive V4" ...)<br />
	`--det`                 Show per size-fragment details (default = OFF)<br />
	`--plate`               Show results in plate layout (default = OFF)<br />
