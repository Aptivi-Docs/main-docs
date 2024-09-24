---
description: Upgrading our library in your project
icon: chevrons-up
---

# Upgrade

There are two ways to upgrade our library in your project:

* Using Visual Studio's NuGet package manager
* Manual upgrade

## Visual Studio's NuGet package manager

If you're using Visual Studio to build your project, it provides you an easy way to install NuGet packages, such as our libraries, into your project. This is easy and straightforward. In order to upgrade a NuGet library to your project, follow the steps:

1.  Open Visual Studio to a project that you want to upgrade our libraries.\


    <figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>
2.  Right click on either the project or the `Dependencies` entry beneath the project in the Solution Explorer pane and select `Manage NuGet packages...`\


    <figure><img src="../../.gitbook/assets/{1131B26C-7EEF-4E37-AC07-E1A4F2EE0512}.png" alt=""><figcaption></figcaption></figure>
3.  Click on `Updates`. Then, select the desired library you'd like to upgrade, such as Terminaux.\


    <figure><img src="../../.gitbook/assets/{32550B1A-A355-40AF-9383-A0AEFB0F694F}.png" alt=""><figcaption></figcaption></figure>
4.  Click on any of the libraries that show up in the search results, and click on `Update`.\


    <figure><img src="../../.gitbook/assets/{9FAF0EE6-0BB7-4ECC-9AFA-C4766550425E}.png" alt=""><figcaption></figcaption></figure>
5.  If any package asks for your acceptance of the license, read the license contained by clicking on their license names, then click on `I Accept`.\


    <figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>
6.  The package is upgraded! Verify by expanding the `Dependencies` entry beneath the project and expanding the `Packages` entry.\


    <figure><img src="../../.gitbook/assets/{F29812C2-C46C-404F-A3E7-29B9962D074D}.png" alt=""><figcaption></figcaption></figure>

## Manual upgrade

If you'd like to manually upgrade a NuGet package to a project with your favorite editor or if you're unable to use Visual Studio for some reason, you can use this upgrade method. However, this method comes in two ways:

* Visual Studio
* Text editor

### Visual Studio

If you are using Visual Studio, follow these steps:

1.  Open Visual Studio to a project that you want to upgrade our libraries.\


    <figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>
2.  Double click on the project as shown in the Solution Explorer pane\


    <figure><img src="../../.gitbook/assets/{A6753112-7AC5-4B42-89F4-034207641237}.png" alt=""><figcaption></figcaption></figure>
3.  Look for the `PackageReference` property that targets a specific library (for example, Terminaux) and change the `Version` attribute (replace `5.3.0.1` with the desired version of the library)



    ```xml
    <ItemGroup>
      <PackageReference Include="Terminaux" Version="5.3.0.1" />
    </ItemGroup>
    ```


4.  Save the project file. It should automatically upgrade the required packages. If, however, the package restoration didn't automatically start, right-click on the solution and select `Restore NuGet Packages`.\


    <figure><img src="../../.gitbook/assets/{0DB138E6-B3F0-4481-895D-38F100E9130A}.png" alt=""><figcaption></figcaption></figure>

### Text editor

If you are using your favorite text editor, such as Visual Studio Code or Sublime Text, follow these steps:

1.  Open the file explorer and navigate to the target project directory that contains the project file (not the solution `.sln` file)\


    <figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>
2.  Right-click on the project file -> `Open With` -> your favorite text editor\


    <figure><img src="../../.gitbook/assets/{3BB11ECE-4C20-44EC-8A5B-81559D2E858C}.png" alt=""><figcaption></figcaption></figure>
3.  Look for the `PackageReference` property that targets a specific library (for example, Terminaux) and change the `Version` attribute (replace `5.3.0.1` with the desired version of the library)



    ```xml
    <ItemGroup>
      <PackageReference Include="Terminaux" Version="5.3.0.1" />
    </ItemGroup>
    ```


4.  Save the project file. Then, open the terminal emulator in your preferred way and execute `dotnet restore`.\


    <figure><img src="../../.gitbook/assets/{43845A85-8286-4B3E-9F16-38E6BD6B68F0}.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
This also applies to terminal-based text editors, such as `vim`, though you'll have to open the terminal emulator beforehand in order to be able to use them.
{% endhint %}
