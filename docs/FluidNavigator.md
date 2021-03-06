# FluidNavigator API
The Fluid Navigator supports almost the same API as the StackNavigator in React Navigation.

## Configuring screens
To set up and configure the different screens available in the navigator, use the regular route config API from StackNavigator:

```javascript
const Navigator = FluidNavigator({
  home: { screen: HomeScreen },
  register: { screen: RegisterScreen },
  finish: { screen: FinishScreen },
});
```

Where each screen is a component to render.

## Configuring Transitions
You can configure transitions for the navigator just like with the StackNavigator.

```javascript
const transitionConfig = {
  duration: 1500,
  timing: Animated.timing,
  easing: Easing.easing
};

const Navigator = FluidNavigator({ Screens }, { transitionConfig });
```
