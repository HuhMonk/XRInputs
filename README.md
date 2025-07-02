# XRInputs
A Unity XR Extension that allows you to call inputs from vr controllers easier


# Documentation


To Use XRInputs You Gotta do 
```csharp
using XRInputs;
```

## Actions
If You Want To Call A Function When Action Is Triggered
```csharp
XRInputs.OnThumbStickPressed += OnThumbstickDown;
XRInputs.OnThumbStickPressed += OnThumbStickUp;
XRInputs.OnGripPressed += OnGripDown;
XRInputs.OnGripReleased += OnGripUp;
XRInputs.OnTriggerPressed += OnTriggerDown;
XRInputs.OnTriggerReleased += OnTriggerUp;
XRInputs.OnPrimaryButtonPressed += OnPrimaryDown;
XRInputs.OnPrimaryButtonReleased += OnPrimaryUp;
XRInputs.OnSecondaryButtonPressed += OnSecondaryDown;
XRInputs.OnSecondaryButtonReleased += OnSecondaryUp;
XRInputs.OnMenuButtonPressed += OnMenuDown;
XRInputs.OnMenuButtonReleased += OnMenuUp;
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
