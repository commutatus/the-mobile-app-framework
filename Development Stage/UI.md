# How to build a good looking UI?
This guide will cover the common UI principles to follow while developing a hybrid app. Some of these principles could be carried over to web development as well. 

You should build the UI by following the steps mentioned below:
1. Look at / Understand the design.
2. Break down the design into smaller components.
3. Think about the implementation. Ask yourself about the components/widgets that you'd use to implement each of those smaller components/widgets.
4. Wireframe. This is probably the most important step of UI development. You can make your development a lot easier if you would just take a moment to wireframe the designs. This is a conscious effort when you're starting out. But it becomes a lot quicker, easier and kind of an automatic process once you're familiar with it.
5. Build the skeleton of the UI by putting the **_HTML_** in place. (I mean the component/widget without the styling).
6. Once everything is in place, you can style it to finish off the implementation.

**Points 5 and 6 aren't really neccessary and can be done together. It is a case of personal preference upto an extent. But following this approach when you're starting out helps to de-clutter the process.**

[comment]: # (Need to add images here. Or should I wait and build the web app directly?!)

Here are a few bonus tips:
- Make sure to provide a visual or an auditory feedback on any instance when user interacts with the app.
  For example: the ripple effect on buttons in android.
- Implement your designs while keeping the different widths of different devices in mind.
Remember that you can use absolute height for components like a full-width card, but you will have to use a variable width for them. 
This is because the Y-axis is normally scrollable and is expected to scroll. Thus even if your height is a bit too much, it'll be fine.
In case of the width, since it's variable in different devices and X-axis scroll isn't an expected behaviour save a few cases, it might overflow the screens.
- Understand whether a component needs absolute or relative dimensions. 
- Make sure to test on both larger and smaller screen devices. Even normal looking lists on bigger screens get screwed on smaller screens if they're not scrollable. Give special attention to screens which have a text input as the keyboard may render a few components/widgets unreachable.
- Consistent padding and margins.
- Lots of whitespace.
- Sometimes using the same values as in the designs might not produce the same result as in the designs due to the difference in the units. In such cases either ask the designer to use dp units, or if that's not possible, don't be afraid to eyeball it and make it look as similar to the designs as possible.