> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

# KidsSafe for Echizen-city Okamoto

A community map for the Okamoto district in Echizen city, visualizing safety, cultural, and tourism information. Data is managed by the community using simple CSV files.

## Demo

https://code4fukui.github.io/kidssafe-okamoto/

## Features

- **Interactive Map:** Visualizes community data, including:
  - **Safety Spots:** AEDs, Children's Refuges (Kodomo 110-ban), security cameras, and patrol routes.
  - **Hazard Information:** Traffic accident locations.
  - **Cultural & Tourism Sites:** Echizen Washi workshops and local points of interest.
- **Community-Managed:** Data is easily updated using CSV files, editable with tools like Excel, Numbers, or Google Sheets.
- **Customizable:** Supports custom map icons for different data types.
- **Open Source:** Built on the [KidsSafe project by Code for FUKUI](https://github.com/code4fukui/kidssafe/).

## How to Use the Map

### Adding to Your Home Screen
For quick access on your smartphone, you can add this site to your home screen, making it function like an app.

### Changing the Site Language
The map interface language can be switched to support various users.

## Data Management

All map data is stored in CSV files within this repository, allowing for easy community updates.

### 1. Updating Existing Data

1.  Navigate to the data file you want to change (e.g., [aed.csv](aed.csv)).
2.  Download the file to your computer.
3.  Open and edit the file in a spreadsheet application.
4.  Upload the modified file back to the repository's main directory. The map will update automatically.

### 2. Adding a New Data Category

1.  Download the [template.csv](template.csv) file.
2.  Add your new data points, with one location per row.
3.  Save the file with a descriptive name (e.g., `parks.csv`) in CSV UTF-8 format.
4.  Download and edit [index.csv](index.csv), adding a new line to define your category: `Parks,parks.csv,park_icon.png`.
5.  Upload both your new data CSV and the updated `index.csv` to the main directory.

### 3. Adding Custom Icons

1.  Prepare a PNG image, approximately 100x100 pixels, with a descriptive English filename (e.g., `park_icon.png`).
2.  Upload the image to the [icon](icon) folder.
3.  Reference the new icon's filename in `index.csv` or other data files to use it on the map.

## Feedback

- For feedback on this specific map (Okamoto district), please open an [Issue](../../issues).
- For feedback on the underlying KidsSafe application, please use the [KidsSafe Issues](https://github.com/code4fukui/kidssafe/issues).

## License

[MIT](LICENSE)