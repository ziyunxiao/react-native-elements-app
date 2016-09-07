# 🔥🔥🔥 React Native Hackathon Starter Project & UI Toolkit 🔥🔥🔥

![React Native UI Toolkit](http://i.imgur.com/80RWAyT.png)

### Included
- [x] [Buttons](https://github.com/dabit3/react-native-hackathon-starter#buttons)
- [x] Pricing Component
- [x] [Social Icons / Buttons](https://github.com/dabit3/react-native-hackathon-starter#social-icons--buttons)
- [x] [Card component](https://github.com/dabit3/react-native-hackathon-starter#card)
- [x] [React Native Vector Icons](https://github.com/oblador/react-native-vector-icons)
- [x] Form Elements
- [x] Redux
- [x] Tabs ([React Native TabNavigator](https://github.com/exponentjs/react-native-tab-navigator))
- [x] Navigator Setup
- [x] HTML style headings (h1, h2, etc...)

#### Todo Soon
- [ ] Add list element
- [ ] Add list item element
- [ ] Add icons to TextInputs
- [ ] Add Profile Component
- [ ] Add Picker
- [ ] Add Search Bar
- [ ] Add Side Menu

##### Todo Major
- [ ] Separate into separate installable NPM package


# API

## Buttons

![Buttons](http://i.imgur.com/aZNhgFp.png)

```
import Button from 'HSButton'

<Button
  raised
  icon={{name: 'cached'}}
  title='RAISED WITH ICON' />
```

| prop | default | type | description |
| ---- | ---- | ----| ---- |
| buttonStyle | none | object | add additional styling for button component |
| title | none | string | button title | 
| onPress | none | function | onPress method |
| icon | none | object {name(string), color(string), size(number)} | [Material Icon Name](https://design.google.com/icons/) | 
| secondary | false | boolean | secondary button flag |
| backgroundColor | primary color | string (color) | background color of button |
| color | white | string(color) | font color |
| textStyle | none | object | text styling |
| fontSize | 18 | number | font size |
| underlayColor | transparent | string(color) | underlay color for button press |
| raised | false | boolean | flag to add raised button styling |

## Social Icons & Buttons

![Social Icons](http://i.imgur.com/k9jQh2u.png)

```
import SocialIcon from 'HSSocialIcon'

// Icon
<SocialIcon
  type='twitter'
/>

// Button
<SocialIcon
  title='Sign In With Facebook'
  button
  type='facebook'
/>
```

| prop | default | type | description |
| ---- | ---- | ----| ---- |
| component | TouchableHighlight | React Native Component | type of button |
| type | none | social media type (facebook, twitter, google-plus-official, pinterest, linkedin, youtube, vimeo, tumblr, instagram, quora, foursquare, wordpress, stumbleupon) | social media type |
| button | false | boolean | creates button |
| onPress | none | funciton | onPress method |
| iconStyle | none | object | extra styling for icon component ([React Native Vector Icons](https://github.com/oblador/react-native-vector-icons)) |
| style | none | object | button styling |
| iconColor | white | string | icon color |
| title | none | string | title if made into a button |

## Forms

![TextInput](http://i.imgur.com/9idGiXr.png)

```
import FormLabel from 'HSFormLabel'
import FormInput from 'HSFormInput'

<FormLabel containerStyle={styles.labelContainerStyle}>Name</FormLabel>
<FormInput onChangeText={someFunction}/>

```

## Card

![Card Component](http://i.imgur.com/eRaY7Ok.png)

```
import Card from 'HSCard'

<Card
  title='CARD WITH DIVIDER'>
  {
    users.map((u, i) => {}
  }
</Card>
```

| prop | default | type | description |
| ---- | ---- | ----| ---- |
| flexDirection | column | string | flex direction (row or column) |
| containerStyle | none | object | outer container style |
| wrapperStyle | none | object | inner container style |
| title | none | string | optional card title |
| titleStyle | none | object | additional title styling (if title provided) |
| dividerStyle | none | object | additional divider styling (if title provided) |

