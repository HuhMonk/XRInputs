<a href="https://discord.gg/8tuuGjuEE9"><img src="https://img.shields.io/badge/discord-brightgreen.svg?style=for-the-badge&logo=discord&colorA=23272a&colorB=7289da" alt="Discord!"></a>

# Documentation


To Use XRInputs You Gotta do 
```csharp
using XRInputs;
```

## Actions
If You Want To Call A Function When Action Is Triggered : make sure before XRInputs.On(Specify hand Right or Left then the rest)GripPressed
```csharp
XRInputs.OnRightThumbStickPressed += OnRightThumbstickDown;
XRInputs.OnLeftThumbStickReleased += OnLeftThumbStickUp;

XRInputs.OnRightGripPressed += OnRightGripDown;
XRInputs.OnLeftGripReleased += OnLeftGripUp;

XRInputs.OnRightTriggerPressed += OnRightTriggerDown;
XRInputs.OnLeftTriggerReleased += OnLeftTriggerUp;

XRInputs.OnRightPrimaryButtonPressed += OnRightPrimaryDown;
XRInputs.OnLeftPrimaryButtonReleased += OnLeftPrimaryUp;

XRInputs.OnRightSecondaryButtonPressed += OnRightSecondaryDown;
XRInputs.OnLeftSecondaryButtonReleased += OnLeftSecondaryUp;

// only left hand menu button
XRInputs.OnMenuButtonPressed += OnMenuDown;
XRInputs.OnMenuButtonReleased += OnMenuUp;

XRInputs.OnRightControllerDisconnect += OnRightControllerDisconnection;
XRInputs.OnLeftControllerReconnect += OnLeftControllerReconnection;
```
## Callings

### Grip : Side Button

If You Want To Get Grip Button Down (bool)
```csharp
  XRInputs.GetGripDown(XRHand Hand);
```
If You Want To Get Grip Button Up (bool)
```csharp
  XRInputs.GetGripUp(XRHand Hand);
```
If You Want To Get Grip Button Value (float)
```csharp
  XRInputs.GetGripFloat(XRHand Hand);
```
## Trigger : Back Button

If You Want To Get Trigger Button Down (bool)
```csharp
  XRInputs.GetTriggerUp(XRHand Hand);
```
If You Want To Get Trigger Button Up (bool)
```csharp
  XRInputs.GetTriggerUp(XRHand Hand);
```
If You Want To Get Trigger Button Value (float)
```csharp
  XRInputs.GetTriggerFloat(XRHand Hand);
```
### Primary : B Or Y Buttons

If You Want To Get Primary Button Down (bool)
```csharp
  XRInputs.GetPrimaryButtonDown(XRHand Hand);
```
If You Want To Get Primary Button Up (bool)
```csharp
  XRInputs.GetPrimaryButtonUp(XRHand Hand);
```
If You Want To Get Primary Button Touched (bool)
```csharp
  XRInputs.GetPrimaryButtonTouched(XRHand Hand);
```
### Secondary : A Or X Buttons

If You Want To Get Secondary Button Down (bool)
```csharp
  XRInputs.GetSecondaryButtonDown(XRHand Hand);
```
If You Want To Get Secondary Button Up (bool)
```csharp
  XRInputs.GetSecondaryButtonUp(XRHand Hand);
```
If You Want To Get Secondary Button Touched (bool)
```csharp
  XRInputs.GetSecondaryButtonTouched(XRHand Hand);
```
### Thumbstick/Joystick

If You Want To Get Thumbstick Down (bool)
```csharp
  XRInputs.GetThumbstickDown(XRHand Hand);
```
If You Want To Get Thumbstick Up (bool)
```csharp
  XRInputs.GetThumbstickUp(XRHand Hand);
```
If You Want To Get Thumbstick Touched (bool)
```csharp
  XRInputs.GetThumbstickTouched(XRHand Hand);
```
If You Want To Get Thumbstick Axis (Vector2)
```csharp
  XRInputs.GetThumbstickAxis(XRHand Hand);
```

### Menu Button
If You Want To Get Menu Button Clicked (bool)
```csharp
  XRInputs.GetMenuButtonClicked(XRHand Hand);
```
If You Want To Get Menu Button Down (bool)
```csharp
  XRInputs.GetMenuButtonDown(XRHand Hand);
```

### Misc

If You Want To Vibrate Controller (corutine)
```csharp
  StartCoroutine(XRInputs.Vibrate(XRHand,0.15f,0.15f));
```

If You Want To Get Both Grip & Trigger Down (bool)
```csharp
  XRInputs.GetGripAndTriggerDown(XRHand Hand);
```

If You Want To Get Primary Down For A Certain Amount Of Time (bool)
```csharp
  XRInputs.WasPrimaryButtonHeldDownFor(XRHand Hand, float Time);
```

If You Want To Get Secondary Down For A Certain Amount Of Time (bool)
```csharp
  XRInputs.WasSecondaryButtonHeldDownFor(XRHand Hand, float Time);
```
