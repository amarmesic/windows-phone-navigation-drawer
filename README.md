Navigation Drawer Layout for Windows Phone 8.1
==============================================

Control implements Android like navigation drawer layout for Windows Phone 8.1. Created as PCL, compatible with Visual Studio 2013.

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
  <drawerLayout:DrawerLayout x:Name="RootLayout">
        <Grid>
            <!-- Main content goes here -->
        </Grid>
        <Grid>
            <!-- Navigation Drwawer goes here -->
        </Grid>
    </drawerLayout:DrawerLayout>
```

Documentation
--------------

### 1. Properties

* IsDrawerOpened - returns true if drawer opened, else returns false

### 2. Methods

* OpenDrawer - opens the navigation drawer

* CloseDrawer - closes the navigation drawer

### 3. Events
Drawer Layout raises two (self explanatory) events:

1. DrawerOpened - raised when you swipe the drawer to the right or call OpenDrawer

2. DrawerClosed - raises when you swipe the drawer to the left or call CloseDrawer

### Demo & Tutorial

Available at http://blog.amarmesic.net

### NuGet

Navigation Drawer Layout is also available as NuGet Package
https://www.nuget.org/packages/DrawerLayout/

Licence
----

The MIT License (MIT)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

