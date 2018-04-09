# NgDigits

This package make sure avoiding non-digits character for input. NgDigits also support maximum digits and Japanese input.

# Install

`npm install ng-digits --save`

## Usage

### Import NgDigits Module
```javascript
import { BrowserModule } from '@angular/platform-browser';
import { NgModule } from '@angular/core';
import {NgDigitsModule} from 'ng-digits';
import { AppComponent } from './app.component';

@NgModule({
  declarations: [
    AppComponent
  ],
  imports: [
    BrowserModule,
    NgDigitsModule
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }
```

### Integer Number without `,` (eg. 12356)
```html
<input appDigits type="text" name="text" id="text"/>
```
### Integer Number with `,` (eg. 12,356)
```html
<input [appDigits]="[]" type="text" name="text" id="text"/>
```
### Decimal Number (eg. 1,235.62)
```html
<input [appDigits]="['1.2']" type="text" name="text" id="text"/>
```
### Integer Number with maximum digits (eg. 12.356)
```html
<input [appDigits]="['1.3']" maxDigits="5" type="text" name="text" id="text"/>
```
## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/Qolzam/react-social-network/tags). 

## Authors

  - Amir Movahedi
  - See also the list of [contributors](https://github.com/De-Amir/ng-digits/contributors) who participated in this project.

## How To Support
- Fork || Star
## License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/De-Amir/ng-digits/blob/master/LICENSE) file for details.

## Credit

Originally made for [@DefideInc][1] by [@De-Amir][2].

[1]: https://github.com/DefideInc
[2]: https://github.com/De-Amir

