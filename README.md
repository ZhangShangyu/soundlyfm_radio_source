# SoundlyFM Radio Source

This repository contains the radio station data source used by [SoundlyFM](https://soundlyfm.com), a retro worldwide radio player for iOS and macOS.

Most station entries were originally initialized from [radio-browser.info](https://www.radio-browser.info).

## About This Repository

If you use SoundlyFM and would like to:

- add a new country or region
- add new radio stations
- update broken streams
- remove duplicate entries

feel free to open a pull request. Updates from this repository are reviewed regularly and will be synced into the SoundlyFM app.

This dataset is public and not limited to SoundlyFM users. You are welcome to use it in your own app or project as well.

## Data Structure

Each country or region is stored as a JSON file inside `station_source/`.

Example:

```json
[
  {
    "id": "7G2Ark1P",
    "name": "Sample Radio",
    "url": "https://example.com/live.m3u8",
    "tags": ["music", "news"]
  }
]
```

### Field Description

- `id`: A random string used as the station identifier. It can be any value as long as it does not duplicate another `id` in the repository.
- `name`: The display name of the radio station.
- `url`: The stream URL of the station.
- `tags`: A list of station categories, such as `music`, `news`, `traffic`, or `economy`.

## Contributing

Pull requests are welcome for:

- new countries or regions
- new stations
- fixing unavailable streams
- removing duplicates
- improving station metadata

Please try to keep the JSON format consistent with the existing files.
