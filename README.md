# JFontAwesome
Unicode Mapping of all FontAwesome (4.3.0) Icons as static Java class. Use this class in your Java FX projects. Find more information about FontAwesome at http://fortawesome.github.io/Font-Awesome/

# Usage
1. Download current release of FontAwesome and extract fontawesome-webfont.ttf to your resource folder.
2. Load the font in your main class like this:
```java
static {     // load FontAwesome     Font.loadFont(YourApp.class.getResource("Resources/fonts/fontawesome-webfont.ttf").toExternalForm(), 12); }
```
3. Add stylesheet
```css
root {     -icons-color: rgb(61,114,114); }  .icons {     -fx-font-family: FontAwesome;     -fx-font-size: 16px;     -fx-text-fill: black; }
```
4. Add unicode mapping class JFontAwesome to your project
5. Use it like this:
```java
Button button = new Button(); button.setStyle("-fx-font-size: 16px;"); button.getStyleClass().add("icons"); button.setText("FontAwesome Button“); button.setGraphic(new Label(JFontAwesome.ADJUST
));







