# JFontAwesome
Unicode Mapping of all *FontAwesome 4.3.0* Icons as static Java class. Use this class in your Java FX projects. Find more information about FontAwesome at http://fortawesome.github.io/Font-Awesome/

# Usage
1.Download current release of FontAwesome and extract fontawesome-webfont.ttf to your resource folder.

2.Load the font in your main class like this:
```java
static { 
Font.loadFont(YourApp.class.getResource("Resources/fonts/fontawesome-webfont.ttf").toExternalForm(), 12); 
}
```

3.Add stylesheet file "icons_default.css" and add it to a container like ```<BorderPane fx:id="MyBorderPane" stylesheets="@styles/icons_default.css" xmlns="http://javafx.com/javafx/8" xmlns:fx="http://javafx.com/fxml/1">```
```css
root {
    -icons-color: rgb(61,114,114);
}

.icons {
    -fx-font-family: FontAwesome;
    -fx-font-size: 16px;
    -fx-text-fill: black;
}
```

4.Add unicode mapping class JFontAwesome to your project

5.Use it like this:
```java
Button button = new Button(); // add a button to your borderpane or container
button.setStyle("-fx-font-size: 16px;"); // set size of the icon plus text
button.getStyleClass().add("icons"); // add css class
button.setText("Your Awesome Button"); // set text of the button
button.setGraphic(new Label(JFontAwesome.ADJUST)); // add FontAwesome icon
```
