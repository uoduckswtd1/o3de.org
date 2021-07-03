---
title: Audio Rtpc
description: Use the Audio RTPC component to set values at runtime that produce real-time tweaking of sounds in Open 3D Engine.
toc: true
---

The **Audio RTPC** component provides basic [Real-Time Parameter Control (RTPC)](/docs/user-guide/interactivity/audio/atl-default-controls) functionality. An RTPC is a named variable that the audio system can interpret in many different ways. It allows game developers to set the value from the game at run time to produce real-time tweaking of sounds.

## Audio RTPC Component Properties

The **Audio RTPC** component has the following property:

**Default Rtpc**
Enter the name of the audio RTPC to use by default. You can associate any RTPC name with the entity, typically one that is meant to affect a particular trigger.

## EBus Request Bus Interface

Use the following request functions with the EBus interface to communicate with other components of your game.

For more information about using the Event Bus (EBus) interface, see [Working with the Event Bus (EBus) system](/docs/user-guide/engine/ebus).

### SetValue

Sets the value of the default RTPC.

**Parameters**
`value` - Float value of the RTPC

**Return**
None

**Scriptable**
Yes

### SetRtpcValue

Sets the value of the specified RTPC.

**Parameters**
`rtpcName` - Name of the RTPC to set
`value` - Float value to set

**Return**
None

**Scriptable**
Yes