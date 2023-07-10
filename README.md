# QT-PyQt-PySide-Custom-Widgets
Awesome custom widgets made for QT Desktop Applications. Simplify your UI development process. These widgets can be used in QT Designer then imported to PySide code.

# Installation 
First time installer:
```
pip install QT-PyQt-PySide-Custom-Widgets
```
Upgrade/install the latest version:
```
pip install --upgrade QT-PyQt-PySide-Custom-Widgets
```

# Installation Testing
Run the following code to see if the installation was successful.

```python
# Run this from your terminal or create a python file, 
# paste this code, then run
from Custom_Widgets.ProgressIndicator import test
test.main()
```

You should see the following interface:
![Custom Progress bar](https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets/blob/main/images/Screenshot.png?raw=true)

# How to use it.
- Read the full documentation plus video guides [here](https://khamisikibet.github.io/QT-PyQt-PySide-Custom-Widgets/) 

[Watch the tutorial videos here](https://www.youtube.com/watch?v=21Qt9p_F7Ts&list=PLJ8t3BKaQLhPKj9Mx08WAwvz7TGskefbK)

# What is new?
## Version 0.6.2:
- Added support for loading multiple ``JSON Stylesheets``
    By default, the json file named ``style.json`` will be loaded, so no need to specify. The file must me inside the root directory of your project, ``json`` directory, or ``jsonstyles`` directory inside your project folder for it to be automatically loaded.
    
    If you have multiple JSON stylesheet files, then you can apply them to your GUI like this:
    ```python
        ########################################################################
        # APPLY JSON STYLESHEET
        ########################################################################
        # self = QMainWindow class
        # self.ui = Ui_MainWindow / user interface class
        loadJsonStyle(self, self.ui, jsonFiles = {
            "mystyle.json",
            "mydirectory/myJsonStyle.json"
            })
        ########################################################################
    ```
    This feature is helpful especially when you have multiple windows files that will share only some parts of the stylesheet shuch app app title, settings etc.
    
- Toggle logs:
    You can now switch app logs on or off.
    This can be done from a python file:
    ```python
    # Show Logs
    self.showCustomWidgetsLogs = True
    ```
    ```python
    # Hide Logs
    self.showCustomWidgetsLogs = False
    ```
    From the JSON file:
    ```json
    {
    "ShowLogs": true,
    ```
    ```json
    {
    "ShowLogs": false,
    ```

# Sample Images

Analog Gauge Widget

![Analog Gauge Widget](https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets/blob/main/images/analog_qt_widget.png?raw=true)

Responsive Animated GUI

![Resposive PyQt PySide GUI](https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets/blob/main/images/responsive-qt-gui-python-intarface.png?raw=true)

Animated QStacked Widget

![Custom QStacked Widgets](https://github.com/KhamisiKibet/QT-PyQt-PySide-Custom-Widgets/blob/main/images/qstacked.png?raw=true)