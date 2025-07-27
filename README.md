# Coffee Machine Virtual Interface

This project is a computer vision-based virtual interface for a coffee machine, using hand gesture recognition to select options. It overlays webcam input and interactive UI elements on a custom background.

## Features

- Hand gesture detection using [cvzone](https://github.com/cvzone/cvzone) and OpenCV.
- Selection of coffee machine modes and options via hand gestures.
- Visual feedback with icons and progress ellipses.
- Customizable backgrounds, modes, and icons.

## Requirements

- Python 3.7+
- OpenCV (`opencv-python`)
- cvzone (`pip install cvzone`)
- Webcam

## Folder Structure

```
Coffee Machine Virtual Interface/
│
├── main.py
├── Resources/
│   ├── Background.png
│   ├── Modes/
│   │   └── [mode images]
│   └── Icons/
│       └── [icon images]
```

## Setup

1. Clone or download this repository.
2. Place your background image in `Resources/Background.png`.
3. Add mode images to `Resources/Modes/`.
4. Add icon images to `Resources/Icons/`.
5. Install dependencies:
   ```
   pip install opencv-python cvzone
   ```
6. Run the project:
   ```
   python main.py
   ```

## Usage

- Show your hand in front of the webcam.
- Use specific finger gestures to select options:
  - `[0, 1, 0, 0, 0]` for option 1
  - `[0, 1, 1, 0, 0]` for option 2
  - `[1, 0, 1, 1, 1]` for option 3
- Progress is shown as a green ellipse. When selection is complete, the icon appears at the bottom.

## Troubleshooting

- If you see `Failed to capture image from webcam.`, check your webcam connection and ensure no other application is using it.
- Make sure all image resources exist and are readable.
- If the UI does not display correctly, check the image sizes in `Resources`.

## License

This project is for educational
