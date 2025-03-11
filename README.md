# REPOLib Sdk

**Unity editor tools for creating content for R.E.P.O. (using REPOLib).**

## Features

- Registering custom valuables without code
- Registering custom items without code
- Registering custom enemies without code
- Automatic asset bundling and Thunderstore packaging

## Installation

This section assumes you already have a Unity project set up for R.E.P.O. modding.
If not, use a tool like [R.E.P.O. Project Patcher](https://github.com/Kesomannen/unity-repo-project-patcher) first.

**1. Add REPOLib to the project**

- Download REPOLib from Thunderstore ([link](https://thunderstore.io/c/repo/p/Zehs/REPOLib/)).
- Extract the downloaded file.
- Copy `REPOLib.dll` into your project.

> [!TIP]
> To update REPOLib, replace the dll with a newer version.

**2. Add REPOLib-Sdk to the project**

- In unity, go to `Window > Package Manager`.
- Click the `+` button in the top left and choose `Add package from git URL`.
- Enter `https://github.com/ZehsTeam/REPOLib-Sdk.git`.

> [!TIP]
> To update REPOLib-Sdk, go to the Package Manager, click on the package and then `Update`.

## Usage

### Create a mod

- Create a new folder in your project.
- Right click in the folder, then choose `Create > REPOLib > Mod`.
- Fill in the fields on the `Mod` asset:
  - `Name`: the mod's name, as shown on Thunderstore. This can only contain numbers, letters and underscores.
  - `Author`: the name of your Thunderstore team.
  - `Version`: must be in the format `X.Y.Z`.
  - `Dependencies`: REPOLib should always be included.
  - `Website Url`: Optional.
  - `Icon`: must be a 256x256 PNG file.
  - `Readme`: a longer description of the mod, in a separate file. Supports markdown formatting.

> [!TIP]
> You can have multiple mods in the same project, as long as they're in separate folders.

### Create a valuable

- Create a valuable prefab.
  - More documentation is on its way here. For now, use the vanilla valuables as a reference. If you used the patcher, they are located in `Assets/REPO/Game/Resources/valuables`.
- Right click in your mod folder (or any subfolder) and choose `Create > REPOLib > Valuable`.
- Fill in the fields:
  - `Prefab`: A reference to your prefab. The prefab does not have to be in the mod folder.
  - `Valuable Presets`: The valuable presets to register the valuable to. The vanilla values are:
    - `Valuables - Generic`
    - `Valuables - Wizard`
    - `Valuables - Manor`
    - `Valuables - Arctic`

### Create an item
- Create an item prefab.
  - More documentation is on its way here. For now, use the vanilla item prefabs as a reference. If you used the patcher, they are located in `Assets/REPO/Game/Resources/items`.
- Create an `Item` by right clicking and going to `Create > Other > Item`.
  - More documentation is on its way here. For now, use the vanilla items as a reference. If you used the patcher, they are located in `Assets/REPO/Game/Resources/items/items`.
- Right click in your mod folder (or any subfolder) and choose `Create > REPOLib > Item`.
- Fill in the fields:
  - `Prefab`: A reference to your prefab. The prefab does not have to be in the mod folder.

### Create an enemy

- Create an `EnemySetup` by right clicking and going to `Create > Other > Enemy Setup`.
  - As with valuables, use the vanilla ones as reference.
- Right click in your mod folder (or any subfolder) and choose `Create > REPOLib > Enemy`.
- Fill in the fields.

### Export a mod

- Select the `Mod` asset and click `Export` in the inspector.
  - In the window you'll see the associated content files found by REPOLib-Sdk.
- Choose an `Output Path`. If there isn't a folder at the selected path, one will be created.
- Click `Export` and wait. Once finished, a window should appear showing the exported zip file. This file can be uploaded to Thunderstore or locally imported into mod managers.

> [!TIP]
> The export window can also be accessed from `Window > REPOLib Exporter`

## Contribute

Anyone is free to contribute.

https://github.com/ZehsTeam/REPOLib-Sdk

## Developer Contact
**Report bugs, suggest features, or provide feedback:**
- **GitHub Issues Page:** [REPOLib](https://github.com/ZehsTeam/REPOLib/issues)
- **Email:** crithaxxog@gmail.com
- **Twitch:** [CritHaxXoG](https://www.twitch.tv/crithaxxog)
- **YouTube:** [Zehs](https://www.youtube.com/channel/UCb4VEkc-_im0h8DKXlwmIAA)

[![kofi](https://i.imgur.com/jzwECeF.png)](https://ko-fi.com/zehsteam)
