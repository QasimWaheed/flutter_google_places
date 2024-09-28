# flutter_google_places2

This library provides Google places autocomplete widgets for flutter. It uses [google_maps_webservice2](https://github.com/QasimWaheed/google_maps_webservice_v2) library which directly refer to the official [documentation](https://developers.google.com/maps/web-services/) for google maps web service. 

According to https://stackoverflow.com/a/52545293, you need to enable billing on your account, even if you are only using the free quota.


## Installation

In the `dependencies:` section of your `pubspec.yaml`, add the following line:

```yaml
dependencies:
  flutter_google_places2: <latest_version>
```

## Usage

```dart
const kGoogleApiKey = "API_KEY";

Prediction p = await PlacesAutocomplete.show(
                          context: context,
                          apiKey: kGoogleApiKey,
                          mode: Mode.overlay, // Mode.fullscreen
                          language: "fr",
                          components: [new Component(Component.country, "fr")]);
```

#### Examples: 
<div style="text-align: center"><table><tr>
    <td style="text-align: center">
<img src="https://raw.githubusercontent.com/fluttercommunity/flutter_google_places/master/flutter_01.png" height="400">
</td>
<td style="text-align: center">
<img src="https://raw.githubusercontent.com/fluttercommunity/flutter_google_places/master/flutter_02.png" height="400">
</td>
</tr>
</table>
</div>

## Example App

View the Flutter app in the `example` directory.
