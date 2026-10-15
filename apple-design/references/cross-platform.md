# Apple term to framework equivalent

| Apple concept | SwiftUI | UIKit | React Native | Flutter | Web (React / HTML) |
|---|---|---|---|---|---|
| Safe area | `.safeAreaInset`, `ignoresSafeArea` | `safeAreaLayoutGuide` | `SafeAreaView` | `SafeArea` | `env(safe-area-inset-*)` |
| Text styles | `.font(.body)` etc. | `UIFont.preferredFont(forTextStyle:)` | `fontSize` + `allowFontScaling` | `Theme.textTheme` | `rem` units, `clamp()` |
| Dynamic Type | automatic | `adjustsFontForContentSizeCategory` | `allowFontScaling` | `MediaQuery.textScaler` | respect browser zoom, no `px` fonts |
| Semantic colours | `Color.primary`, `.secondary` | `UIColor.label` | `PlatformColor` | `ColorScheme` | CSS custom properties + `prefers-color-scheme` |
| Navigation stack | `NavigationStack` | `UINavigationController` | React Navigation native stack | `Navigator` / go_router | history + back affordance |
| Tab bar | `TabView` | `UITabBarController` | bottom tabs | `BottomNavigationBar` | bottom nav on mobile widths |
| Sheet | `.sheet` | `UISheetPresentationController` | modal, `presentationStyle: pageSheet` | `showModalBottomSheet` | dialog or drawer |
| Alert | `.alert` | `UIAlertController` | `Alert` | `AlertDialog` | `<dialog>` |
| 44pt target | `.frame(minWidth: 44, minHeight: 44)` | `hitTest` or size | `hitSlop` | `minimumSize` | `min-height: 44px` |
| VoiceOver label | `.accessibilityLabel` | `accessibilityLabel` | `accessibilityLabel` | `Semantics(label:)` | `aria-label` |
| Reduce Motion | `@Environment(\.accessibilityReduceMotion)` | `UIAccessibility.isReduceMotionEnabled` | `AccessibilityInfo` | `MediaQuery.disableAnimations` | `prefers-reduced-motion` |
| Spring animation | `.spring()` | `UIViewPropertyAnimator` | Reanimated `withSpring` | `SpringSimulation` | `linear()` easing or a spring lib |
| Keyboard type | `.keyboardType(.emailAddress)` | `keyboardType` | `keyboardType` | `TextInputType` | `type="email"`, `inputmode` |
| Content type | `.textContentType(.oneTimeCode)` | `textContentType` | `textContentType` | `autofillHints` | `autocomplete` |
