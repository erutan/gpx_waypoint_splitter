# GPX Waypoint Splitter

I had a GPX file with more than 15k waypoints I needed to import to a service that only allowed 1k items per upload. This will split a gpx file into multiple files containing however many waypoints you specify.

Thanks Claude!

## Useage

Basic usage (default: 1000 waypoints per file):
`python gpx_waypoint_splitter.py MYFILE.gpx`

If you want to have the base output filename be different from your input, add your desired filename after the input:
`python gpx_waypoint_splitter.py MYFILE.gpx new_name`

You can change how many waypoints per file by passing the number as an argument to the -w flag, 500 in this case:
`python gpx_waypoint_splitter.py MYFILE.gpx -w 500`

If you wanted to output new_name_001.gpx and new_name_002.gpx etc with 2000 waypoints each you'd use the following:
`python gpx_waypoint_splitter.py MYFILE.gpx new_name -w 2000`

## MacOS Notes

You can install Python via the [homebrew](https://brew.sh/) package manager. Unless you create an alias in your shell, you'll need to replace 'python' with 'python3' in the commands above.