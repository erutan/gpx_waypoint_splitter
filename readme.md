# GPX Waypoint Splitter

I had a GPX file with more than 15k waypoints I needed to import to a service that only allowed 1k items per upload. This will split a gpx file into multiple files containing however many waypoints you specify.

Thanks Claude!

```
# Basic usage (default: 1000 waypoints per file)
python gpx_splitter.py tracking_data.gpx

# With custom output prefix
python gpx_splitter.py tracking_data.gpx hiking_segments

# Specifying 500 waypoints per file
python gpx_splitter.py tracking_data.gpx --waypoints-per-file 500
# OR using the short form
python gpx_splitter.py tracking_data.gpx -w 500

# Combining custom prefix and waypoints per file
python gpx_splitter.py tracking_data.gpx hiking_segments -w 2000
```

### MacOS Notes

You can install Python via the [homebrew](https://brew.sh/) package manager. Unless you create an alias in your shell, you'll need to replace 'python' with 'python3' in the commands above.