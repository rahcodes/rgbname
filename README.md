# RGB to Colour Name using Nearest Neighbour
## About
This webpage accessible [here](https://rahcodes.github.io/rgbname/) provides a tool that can identify names of upto __30241__ different colours from a given RGB value. It uses the Nearest Neighbour (NN) approach with Euclidean distance to determine the closest match to RGB values in the dataset.

There's two datasets included in this repository. One is `colours.json` containing __1298__ different colour names, while the other dataset `colours1.json` contains __30241__ different names. The webpage primarily utilizes `colours1.json`.

The dataset for `colours1.json` is sourced from [meodai's color-name](https://github.com/meodai/color-names/). It was obtained as the `colornames.csv` file found on their page, which was then reformatted into `colours1.json` file using this Python [notebook](https://colab.research.google.com/drive/1RywAYP84f83SpQTJpsCEPNuoIfqJexKu?usp=sharing).

The dataset for `colours.json` is sourced from [here](https://www.kaggle.com/datasets/avi1023/color-names).
## JSON Dataset Structure
The structure of `colours1.json` is as follows:
```javascript
[
    {
        name: "Colour Name",
        rgb: [100, 100, 100]
    },
    {
        name: "Colour Name 2",
        rgb: [200, 200, 200]
    },
]
```
And the structure of `colours.json` is as follows:
```javascript
{
    colours: [
        {
            name: "Colour Name",
            red: 100,
            green: 100,
            blue: 100
        },
        {
            name: "Colour Name 2",
            red: 200,
            green: 200,
            blue: 200
        },
    ]
}
```
## Demo
![rgb_name_demo](https://github.com/rahcodes/rgbname/assets/39433922/4b066279-2fdb-453d-92c0-9f37657cbaf7)
