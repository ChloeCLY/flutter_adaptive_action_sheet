# Adaptive action sheet (Developers Preview)

A action bottom sheet that adapts to the platform (Android/iOS).

iOS | Android
--- | ---
<img width="520" alt="n1" src="https://github.com/Daniel-Ioannou/flutter_adaptive_action_sheet/blob/master/assets/ReadMe%20iOS%20Screenshot.png"> | <img width="497" alt="n2" src="https://github.com/Daniel-Ioannou/flutter_adaptive_action_sheet/blob/master/assets/ReadMe%20Android%20Screenshot.png">

## Getting Started

 Add the package to your pubspec.yaml:

 ```yaml
 adaptive_action_sheet: ^1.0.0
 ```
 
 In your dart file, import the library:

 ```Dart
import 'package:adaptive_action_sheet/adaptive_action_sheet.dart';
 ``` 
  Instead of using a `showModalBottomSheet` use `showAdaptiveActionSheet` Widget:

  ```Dart
showAdaptiveActionSheet(
   context: context,
   actions: <BottomSheetAction>[
      BottomSheetAction(title: 'Item 1', onPressed: () {}),
      BottomSheetAction(title: 'Item 2', onPressed: () {}),
      BottomSheetAction(title: 'Item 3', onPressed: () {}),
   ],
);
```

### Parameters:
#### showAdaptiveActionSheet:
* `actions`: The Actions list that will appear on the ActionSheet. (required)
#### BottomSheetAction:
* `title`: The string that will appear in the title bar of the action item. (required)
* `onPressed`: The callback that is called when the action item is tapped. (required)
