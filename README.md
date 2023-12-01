# Briquetales

A new Flutter project.

## Getting Started

### Steps to run this project.

- Install Xcode:
   Make sure you have Xcode installed on your Mac. You can download it from the Mac App Store.

- Open Xcode:
   Launch Xcode and make sure to open it at least once to accept any license agreements and complete the initial setup.

-Configure Flutter for iOS:
   Open Terminal and navigate to your Flutter project's root directory. Run the following command to create the necessary files for iOS:

   ```bash
   flutter create .
   ```

- Check Dependencies:
   Ensure that your Flutter project doesn't have any dependencies or plugins that are specific to Android.

- Update Podfile:
   Navigate to the `ios` directory within your Flutter project using Terminal and open the `Podfile` using a text editor (e.g., nano, vim, or VSCode).

   ```bash
   cd ios
   nano Podfile
   ```

   Update the `platform` line to ensure it targets the latest iOS version:

   ```ruby
   platform :ios, '10.0'
   ```

   Save and close the file.

- Install Dependencies:
   Still in the `ios` directory, run:

   ```bash
   pod install
   ```

- Open Xcode Workspace:
   Open the `.xcworkspace` file in the `ios` directory using Xcode.

- Configure Signing:
   In Xcode, select your project in the left sidebar, go to the "Signing & Capabilities" tab, and configure the Team and Bundle Identifier under "Signing."

- Build Project:
   Build the project in Xcode (Product > Build).

- Select Device:
    Connect your iOS device to the Mac. In Xcode, select your connected device as the build target.

- Run the App:
    Run the app on your device. This step is crucial as it ensures the app is properly signed and packaged.

- Archive the Project:
    Once the app runs successfully on the device, go to Product > Archive in Xcode.

- Distribute IPA:
    In the Organizer window, select the archived build and click on "Distribute App." Choose "Development" or "Ad Hoc" depending on your needs.

- Follow the Wizard:
    Follow the distribution wizard, and Xcode will generate the IPA file.

- Share or Save IPA:
    After the distribution process, you can save or share the IPA file as needed.

