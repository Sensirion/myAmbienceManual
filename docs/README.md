# Introduction

## About this document
![Pinout](images/app_icon.png ":size=10%")

This is a short introduction to the Sensirion MyAmbience app for iOS and Android devices. 
MyAmbience is used together with the official Sensirion Demonstrators which can be found on the [Sensirion website](https://sensirion.com/search?q=gadget) as well as 3rd party do-it-yourself demonstrators.

The Manual refers to MyAmbience version 3.5 and newer. 

## Supported Demonstrators

Most of the following demonstrators are not publicly available for sale. We do however sell and hand out some demonstrators during our marketing events and at trade
fairs.
Visit us at our next trade fair near you. Go to [our website](sensirion.com/fairs-events) to check our upcoming events.

The following Demonstrators are currently supported:

### SCD4x CO2 Gadget
![SCD4x CO2 Gadget](images/my_co2_gadget.png ":size=30%")

Learn more about the SCD4x and the SCD4x CO2 Gadget at [our website](https://sensirion.com/products/catalog/SCD4x-CO2-Gadget)

### SHT4x Smart Gadget
![SHT4x SmartGadget](images/sht4x_gadget.png ":size=30%")

Learn more about the SHT4x and the SHT4x SmartGadget at [our website](https://sensirion.com/products/catalog/SHT4x-Smart-Gadget)

### SHT31 SmartGadget
![SCD4x CO2 Gadget](images/sht31_gadget.png ":size=30%")

This is deprecated but still compatible with the MyAmbience app.
Learn more about the SHT3x and the SHT31 SmartGadget at [our website](https://sensirion.com/products/catalog/SHT31-Smart-Gadget)

### Nubo Air Monitoring system
![Nubo Air Monitoring system](images/nubo.png ":size=30%")

Learn more about Nubo at [our website](https://sensirion-connected.com/solutions/nubo-sphere/)

### Do-it-yourself Demonstrators
![Do it yourself](images/esp_based.png ":size=30%")

You can create your own demonstrators and connect them to MyAmbience!
Learn how to create your own on [our Github page](https://github.com/Sensirion/arduino-ble-gadget)!


# Getting Started

## Download MyAmbience for your OS

### Apple iOS:
You can download the iOS MyAmbience app through the oficial Apple App Store through the following link or QR code:

[MyAmbience iOS App](https://apps.apple.com/us/app/sensirion-myambience/id1529131572#?platform=iphone) 

![MyAmbience iOS App](images/qrcode_apps.apple.com.png ":size=25%")

### Google Android:
You can download the Android MyAmbience app through the oficial Google Play Store through the following link or QR code:

[MyAmbience Android App](https://play.google.com/store/apps/details?id=com.sensirion.myam) 

![MyAmbience Android App](images/qrcode_play.google.com.png ":size=25%")

## Requirements and Permissions

The following permissions need to be set so that MyAmbience can detect surrounding demonstrators:

- Bluetooth on your device needs to be enabled and the app needs to have permissions for bluetooth.
- On Android devices location permissions need to be given in addition. We do not store location information, however this is required by the bluetooth functionality since on some Android versions these are coupled.
- In case you would like to get notifications when you download data from the demonstrators devices and export data, please allow notifications for MyAmbience.
- The gadget needs to be in a range of 10-15 meters from the mobile. This varies between devices, however, this is the typical operating distance of bluetooth devices.

# Using MyAmbience

## Main Screens

MyAmbience is divided into three main screens:

- [Dashboard](#dashboard)
  
- [Plots](#plots)
  
- [Menu](#menu)
  


## Dashboard
![Dashboard](images/Dashboard.PNG ":size=20%")

### Gadget Overview

The main screen of MyAmbience offers an overview of all the nearby active gadgets. Normally gadgets within a 10-15m radius can be found.

Each gadget has its own "card" which shows an overview of all the available sensor signals. The colors of the signals vary depending on the value and how "high or low" this is. An example is shown in the image below:

![Gadget Overview](images/Gadget%20Overview.PNG ":size=20%") 

The gadgets are listed in an alphabetical order and the user can scroll down to see all of the available gadgets.

### Single Gadget Focus view
If you want to focus only on one gadget, you can tap on the card and a focused view emerges which shows the available values for each gadget. Tapping on a value card opens the plot for this signal. Additionally, there is a set of statistics for the previous 24 hours such as minimum and maximum value as well as an average. An example of the focused view is shown in the image below:

![Focus View](images/Focus%20View%20SHT.PNG ":size=20%") 

### Favorite Gadgets

MyAmbience allows you to mark "Favorite" gadgets. Favorite gadgets will always show on the top of the gadget list. 

To favorite a gadget, simply tap the heart icon on the bottom right of each gadget card as shown in the picture below:

![Favorite Gadgets](images/Favorite%20gadgets.PNG ":size=20%") 

The favorite settings are persistent even if your gadget is not in reach. The next time you are close to your gadget it will show up on top!

### Gadget Settings

You can configure certain aspects of your gadget! By tapping the cog wheel icon next to the favorites icon on the bottom right you go into the settings view. An example is shown below for the SCD4x CO2 Gadget:

![Settings View](images/Settings.PNG ":size=20%") 

Through the settings view you can:
- Update the firmware of your gadget. The app will automatically detect a firmware which needs to be updated and will allow you to start the update.
- Change the name of your gadget. Please note, that this will change the gadget name only for your own device and not overall of the gadget
- See the battery percentage, the available logging memory and adjust the logging interval 
- (CO2 Gadget Only) Adjust the LED Brightness
  - Turn on/off the LED by tapping on the light bulb on the bottom right
- (CO2 Gadget Only) Perform a Forced Recalibration


## Plots


The plot view is very useful to understand the historical data from your environment. For example how the CO2 concentration is when you sleep at night with closed doors and windows or what the relative humidity is in the summer versus the winter.

### Gadget Selection

To see the plot for a gadget you can select it from the buttons in the bottom of the app. Selected gadgets show in green.

Please note: By default a single tap on a gadget adds it in the list of the gadgets. If you would like to focus on the plot of only one gadget you have to long press the gadget button 

![Plots](images/Plot.PNG ":size=20%")


### Plot Interaction
The plot interaction is intuitive and simple to allow the users to focus on the signal values.

The x axis of the plots always show the time that the data was captured by the gadget. By using two finger gestures and pinching you can zoom in/out in the x axis while the y axis is automatically adjusted so that the whole signal(s) is in the view.

In case of multiple selected gadgets both plots are shown and the y axis is automatically adjusted so that it fits both plots.

By using the signal buttons above the plot area you can switch between the various signals and see their values.

#### Full Screen view

A new feature is the ability to go into full screen mode so that you can focus only on the plot at hand.

By tapping the arrow button just below the plot you enter the fullscreen mode as shown in the image below:

![Fullscreen mode](images/Fullscreen.PNG ":size=20%")

#### Time ranges and live mode

MyAmbience gives you the ability to quickly jump between different time ranges by tapping the relevant button below the plot area. This is particularly useful when you want to contrast data between multiple days or weeks to identify patterns in your indoor environment. 

![Time ranges](images/Time%20ranges%20and%20single%20plot.PNG ":size=20%")

A new mode in MyAmbience is the live mode, this will automatically move the plot to always show the new values and it will retain the current time range. As soon as you manually move the plot, the app goes out of live mode and allows the user to see the previous measurements.

#### Data down sampling

Depending on the X-Axis range selected the original data is down sampled. This allowes for performant plotting. You can disable the data down sampling for the plot in the [App Settings](#app-settings).

## Fetching stored data from gadget

While the app is active, live data is captured and stored for all gadgets in range. However, most of the gadgets have internal memory which allows them to log the data and send it to MyAmbience upon request. The logging interval on the gadget device can be changed in the [Gadget Settings](#gadget-settings).

There are two ways to initiate a data download:

- In the Plot screen, press the download icon on the top right which will take you to the download view and start fetching data for all selected gadgets.
- In the Dashboard, press the download icon on the gadget card. This will take you to the download view and start fetching data for this gadget.

The app needs to firstly connect to the gadget and then download the previously recorded data.

It is recommended that you are in close proximity of the gadget when trying to fetch the data.

![Download Data](images/DownloadsOverview.png ":size=20%")

On the download screen, you are informed about the download in progress. 
To cancel a running download, swipe the card to the left. Any data already downloaded is discarded.

As the download of data might take some time, you can leave the download view and the data download will continue in background. You are informed about
the download progress with a notification. Additionaly, the download state is visualized with an icon in the bottom right of the gadgets's dashboard card.
You can go back to the download view by tapping on that button at any time or by using the download button in the Plot screen. 

![Download Complete](images/DownloadsComplete.png ":size=20%")

When a download is finished, the download view shows you the number of samples downloaded and their time range. You can explore the data in the Plot screen.

When a download failed or was interrupted due to lost or weak Bluetooth Connection, it is visualized in the download view. You can retry the download by pressing the refresh button on the right of a download card.

If you do no longer want to keep the download card in the list, you can dismiss the card by swiping to the left or removing all downloads not in progress anymore with the "Dismiss finished" button in the bottom right corner of the screen.


## Export and Share data

You can export the stored data from your gadgets.

To select the data to export, you have two options:

Use the share button on the top right in the Plot screen to export data for all selected gadgets.

![Share Data from Plot](images/Share.PNG ":size=20%")

Go to the [Manage Gadgets](#manage-gadgets) Menu, select one or more gadgets and choose the export option.

![Share Data from Manage Gadgets](images/ShareFromManage.png ":size=20%")

Once you have started a export, the Share exported data screen will open and show the progress of the export.
You can leave this screen and the export will continue in the background. You will be notified once the export is finished.
To navigate back to the export screen, use the [Share exported data](#share-exported-data) menu.

![Share exported data](images/Export%20Overview.PNG ":size=20%")

Once the export is finished, you can share your data by tapping on the share button on the card.

The exported data persists until you dismiss it by swiping the entry to the left or you close the app.

The data is exported in an EDF file format. The EDF format is CSV compatible which means you can open it with Excel or any other editor capable of handling CSV.
The EDF files are compatible with ControlCenter and Dataviewer (Sensirion Evaluation Software), so that you can plot your gadget data in Dataviewer.

The timestamps are displayed in your local time. If you want to have timezone offsets included with your timestamps, you can enable this in the app settings.
However, this makes it more difficult to display the data in Excel as it can't handle offsets automatically.

For more information about EDF files please visit the [ControlCenter Manual](https://sensirion.github.io/ControlCenterManual/#/?id=edf-files-explained).


## Menu
![Menu](images/Menu.PNG ":size=20%")

### App Settings

In the app settings you can adjust the general settings of MyAmbience:

- Adjust the measurement system from measuring in degrees Celcius or degrees Fahrenheit or Kelvin
- Select which computed signals will be displayed if the measured signals are available. To learn more about the computed signals for the SHT4x SmartGadget visit the link [here](https://sensirion.com/resource/application_note/sht/glance).
- Select whether you want timezone offsets added to the timestamps in the exported data.
- Select whether you want to down sample live data before storing to the data base, see [Live data down sampling](#live-data-down-sampling) for details.
- Select whether the data displayed in the plot is down-sampled for better performance. Down sampling rate depends on the currently selected X-Axis range.
- Opt in/out in our analytics
- Connect to a Nubo device

#### Live data down sampling

Depending on the gadget, the live data updates every few seconds. As usually there is no such high data resolution needed for the history data, this options allows you to down sample the live values before perstisting. Activating the down-sampling reduces storage consumption and also helps to keep the app performant. The persisted data is used for statistic in [Single Gadget Focus view](#single-gadget-focus-view), plot [Plots](#plots) and data export [Data Export](#export-and-share-data). Note that the plot shows the full resolution for the live data that was traced in the current app session.

The down sampling resolution is set with following logic:
- If a gadget supports data logging, the data logging interval set on the gadget is used as down sampling interval. It is limited to a maximum of 10 minutes. See in the [Gadget Settings](#gadget-settings) to check if your gadget supports data logging. The currently set logging interval is fetched from the gadgets upon discovery and cached in the app.
- Default down sampling interval is 1 minute. This is applied if the gadget does not support data logging.

### Manage Gadgets

![Manage Gadgets](images/Manage%20gadgets.PNG ":size=20%")

The Manage gadgets area allows you to see all the previously detected gadgets and perform certain actions with their data. Actions include:

- Load the gadget as an offline device to visualize the data
- delete the gadget and its data
- delete the data of the gadget
- Select multiple gadgets
- export data of the gadget

There are three different states a gadget can be:

- Active: denoted in green color
- Connecting: Denoted in light blue color
- Not found (Gadget is out of reach): Denoted in grey color

### Share exported data

For more details about how to start a data export, please refer to [Export and Share data](#export-and-share-data) section.

## Support and Feedback

A really important aspect of our mindset at Sensirion is to actively
solve problems of our users, therefore gathering feedback and supporting
our users is of outmost importance to us.

If you request any type of additional support please do not hesitate to
contact us by filing an issue on our [developer support page](https://sensirion.atlassian.net/servicedesk/customer/portal/1) mentioning MyAmbience as a product.

# Appendix
## Privacy Policy and information we collect

### Introduction

This privacy policy outlines details about the data processing in relation to the Sensirion Smart Gadget (“Device”) and the Sensirion MyAmbience mobile application thereto (“App”). In addition, we adhere to the general, Sensirion Privacy Notice, and you have all rights mentioned therein.

The Device allows tracking of environmental data, such as temperature, humidity and carbon dioxide. These data are saved locally onto the Device. The Device has a Bluetooth Low Energy (BLE) module which — when switched on — allows other Bluetooth enabled devices in the vicinity to connect to the Device and show current measured values as well as download saved data.

The Sensirion App allows the user to connect a mobile phone or tablet to the Device and show current measured values as well as download saved data.

The use of MyAmbience (by Sensirion AG) requires that we, Sensirion AG, collect, process, and store certain information about you and, as the case may be, your company. This includes information you provide to us, information we collect automatically, and information we receive from other sources. Such information may include personal data protected under data protection laws.

Please see the full Sensirion Privacy Notice located at https://sensirion.com/legal-notice/privacy-notice/ for the detailed Sensirion data privacy policy.

This Myambience Privacy Notice is in addition to the Sensirion Privacy Notice and highlights what we consider most relevant for you to know regarding the use of MyAmbience:

 

### The Information we collect

Information you provide to us, this includes
Information from actions you take. We collect information about your use of and activities on the services. This includes the type of sensors you connect, the measurement duration, and other related actions.
Other information you provide directly to us. You may have the option to submit additional information as you use MyAmbience. For example, you may participate in surveys where you can provide feedback on the product, which requires that you provide additional information about your device, yourself or your company.
Information we collect automatically, this includes
Information about your device. We collect information about the device you are using to access the services. This includes information like operating system information, screen size and browser information.
Information about your use of the apps or websites. We collect log and event information related to how and when you use our services (such as the sensors connected).
Information we receive from other sources, including third parties, and combine that information with the other information we have about you.
We use Mixpanel Analytics, an analytics service provided by Mixpanel Inc. (“Mixpanel”). For more information on how Mixpanel uses this data, please visit Terms of Use | Legal | Mixpanel.
In order to collect the above mentioned information, we rely on the default services provided by the Android and iOS operating systems.
 

### How we use your information

We use your information for the following purposes:

To provide customer service. We use your information to respond to your questions about our products and services, and to investigate bugs or other issues.
To report on our company’s performance. We use your information to track the fundamental metrics of our business, to perform financial reporting, to respond to regulatory obligations, and to debug billing issues.
To improve our services. We use your information to help us understand how users interact with our services, what features or products users may want, or to otherwise understand and improve our services. This includes information about how you use our services. As discussed in the ”How to control your privacy” section below, you can control whether your data is used for these purposes.
With your consent
We may also collect and use personal information with your consent. You can revoke your consent at any time (mostly through our services directly), though note that you might not be able to use services or features that require collection or use of that personal information.
 

### How to control your privacy

You can restrict our ability to use your data to improve our products. If you turn off the “Send Usage Statistics” setting under settings, we will stop collecting and using certain event and log information to help us understand how users use our services, what features or products they may want, or to otherwise improve our services.
You can request for your data to be deleted by sending an email to privacy@sensirion.com and by supplying your anonymous identifier found under the application settings
Please see the full Sensirion Privacy Notice located at https://sensirion.com/legal-notice/privacy-notice/ for an overview of the rights you have as a data subject.
 

### How we share your information

Aggregated or de-identified information. We may share information about you that has been aggregated or anonymized such that it cannot reasonably be used to identify you. For example, we may share aggregated user statistics in order to describe our business to partners or the public.
