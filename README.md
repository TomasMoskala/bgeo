# bgeoWARNING in C:\aa\TESTS\bgeo\src\test.ts is part of the TypeScript compilation but it's unused.
Add only entry points to the 'files' or 'include' properties in your tsconfig.

WARNING in C:\aa\TESTS\bgeo\src\environments\environment.prod.ts is part of the TypeScript compilation but it's unused.       
Add only entry points to the 'files' or 'include' properties in your tsconfig.

import { NavController, Platform } from 'ionic-angular'; // ionic-angular not working, shold be '@ionic/angular'

module "cordova-background-geolocation-lt"
All imports in import declaration are unused.ts(6192)
" should be ' (quotemark)tslint(1)

I keep my decorator
@Component({
  selector: 'app-home',
  templateUrl: 'home.page.html',
  styleUrls: ['home.page.scss'],
})

added to home.page.ts
  public myLocation: Location;

added
  onLocation(location: Location) {
    this.myLocation = location;

changed template home.page.html
<ion-content [fullscreen]="true">
  <ion-label>Location {{ myLocation }}</ion-label>
</ion-content>

browser error
core.js:6228 ERROR Error: Uncaught (in promise): TypeError: Cannot read property 'onLocation' of undefined
TypeError: Cannot read property 'onLocation' of undefined
    at Function.push../node_modules/cordova-background-geolocation-lt/src/ionic/index.js.BackgroundGeolocation.onLocation (index.js:181)
    at HomePage.configureBackgroundGeolocation (home.page.ts:27)
