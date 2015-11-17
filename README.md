Navigation Drawer Layout for Windows Phone 8.1
==============================================

'One Drive like' Navigation Drawer Layout for Windows Phone 8.1.

![Navigation Drawer](http://amarmesic.net/img/navdrawer.gif)

Features
----
* swipe support
* landscape and RTL support (@konradbartecki)

How to Use
----

* Clone (download) the project

* Add the project (or just the .cs file) to your existing solution

* Add reference in your Windows Phone project

* In your MainPage.xaml, add a namespace
```sh
 xmlns:drawerLayout="using:DrawerLayout"
```

* Replace the root Grid layout with the DrawerLayout

* Create two child Grid controls inside the DrawerLayout. First control will contain the main content and the second will contain the navigation drawer. Your MainPage.xaml code should look like this:

```sh
  <drawerLayout:DrawerLayout x:Name="DrawerLayout">
        <Grid>
            <!-- Main content goes here -->
        </Grid>
        <Grid>
            <!-- Navigation Drwawer goes here -->
        </Grid>
    </drawerLayout:DrawerLayout>
```

The final step is to initialize the layout in your MainPage constructor:

```sh
 public MainPage()
        {
            this.InitializeComponent();
            DrawerLayout.InitializeDrawerLayout();
        }
```

Documentation
--------------

### 1. Properties

* IsDrawerOpened - returns true if drawer opened, else returns false.

### 2. Methods

* InitializeDrawerLayout - initializes the drawer layout. Method must be called inside constructor.

* OpenDrawer - opens the navigation drawer.

* CloseDrawer - closes the navigation drawer.

### 3. Events
Drawer Layout raises two (self explanatory) events:

1. DrawerOpened - raised when you swipe the drawer to the right or call OpenDrawer.

2. DrawerClosed - raises when you swipe the drawer to the left or call CloseDrawer.

### Demo & Tutorial

Demo app on Windows Phone Store:
[http://www.windowsphone.com/s?appid=d0264913-cfa2-4273-91c5-8372a5347084](http://www.windowsphone.com/s?appid=d0264913-cfa2-4273-91c5-8372a5347084 "Windows Phone Store Demo App")

Tutorial available on [http://www.c-sharpcorner.com/UploadFile/cb386b/implementing-navigation-drawer-for-windows-phone-8-1/](http://www.c-sharpcorner.com/UploadFile/cb386b/implementing-navigation-drawer-for-windows-phone-8-1/ "C Sharp Corner")

### NuGet

Navigation Drawer Layout is also available as NuGet Package
[https://www.nuget.org/packages/DrawerLayout/](https://www.nuget.org/packages/DrawerLayout/ "NuGet Package")

### Windows Phone 8 Support

For Silverlight version, check out the port on https://github.com/jgannaway/windows-phone-navigation-drawer

Credits: Jeremy Gannaway (https://github.com/jgannaway)

Licence
----

[http://opensource.org/licenses/MIT](http://opensource.org/licenses/MIT "MIT Licence")
