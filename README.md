# Home Assistant Blueprints

A curated collection of **Home Assistant** automation blueprints to help you save energy, improve comfort, and automate common household tasks.

![Blueprints](https://img.shields.io/badge/blueprint-home--assistant-blue)

## 🌟 Getting Started

This repository contains the following Home Assistant blueprints:

| Blueprint Filename                       | Description                                                                                         | Notes                                                                                         |
|------------------------------------------|-----------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| `ac_efficency_and_notify.yaml`      | Notifies a mobile user when the AC is running and a window/door is open, waits for a response, then shuts off the AC (optional follow-up voice alert). | Tested only for android devices, not tested what happens when multiple mobile devices choose different options in their notifications. |
<!-- Add new blueprints here as you publish them -->

## 📂 Installation

You can add a blueprint to your Home Assistant in one of two ways:

1. **Local copy**  
   - Copy the blueprint YAML file into your configuration, for example:  
     ```
     config/blueprints/automation/<custom_folder>/<blueprint_name>.yaml
     ```
   - In Home Assistant UI go to **Settings → Automations & Scenes → Blueprints → Import Blueprint**, then browse and select the file you just added. e.g
     ```
     <custom_folder>/<blueprint_name>.yaml
     ```

2. **Import by URL**  
   - In Home Assistant UI go to **Settings → Automations & Scenes → Blueprints → Import Blueprint**.  
   - Paste the raw URL of the blueprint file (e.g. `https://raw.githubusercontent.com/antmarpen/home-assistant-blueprints/refs/heads/main/ac_efficency_and_notify.yaml`) and click **Preview → Import**.

Once imported, you can create an automation from the blueprint via **Settings → Automations & Scenes → Create Automation → Use Blueprint**.  


## ⚙️ Example of Usage

1. **Create a new automation** and choose **“Use Blueprint”.**

2. Select **AC Efficiency: Auto-Shut & Notify**.

3. Fill in the inputs:

    - **Air Conditioner** (your climate entity)

    - **Windows & Doors** (your door/window binary_sensors)

    - **Companion App** device(s), timeouts, and messages

    - (Optional) voice notification services and message template

4. Save and test — when a window/door opens with the AC on, you’ll get a notification!

## 🚀 Contributing
Contributions are welcome! To add your own blueprint:

1. **Fork** this repository & create a feature branch.

2. Add your .yaml blueprint under the root or in a subfolder.

3. Update this **README.md** with your blueprint name & description.

4. Open a **Pull Request** — I’ll review and merge.

Please follow the [Home Assistant Blueprint Style Guide](https://www.home-assistant.io/docs/blueprint/style/) for best practices.

## 🤝 Support & Feedback
Found an issue? Open an Issue in this repo.

Have ideas? Let’s discuss on the PR or in the Home Assistant community: https://community.home-assistant.io


    Made with love by antmarpen for the Home Assistant community.