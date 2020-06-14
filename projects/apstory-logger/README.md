[![Build status](https://apstory.visualstudio.com/ApStory/_apis/build/status/apstorymq-client-angular)](https://apstory.visualstudio.com/ApStory/_build/latest?definitionId=25)

# Apstory Application Insights Logger

## Installation

To install this package run `npm i apstory-logger`.

## Usage

Add the following to `app.module.ts`

```javascript
import { ApstoryLoggerModule, ApstoryLoggerService } from 'apstory-logger';
import { BrowserModule } from '@angular/platform-browser';
import { NgModule } from '@angular/core';
import { HttpClientModule } from '@angular/common/http';
import { AppComponent } from './app.component';

@NgModule({
  declarations: [
    AppComponent
  ],
  imports: [
    BrowserModule,
    HttpClientModule,
    ApstoryLoggerModule.forRoot('instrument key here', 'logging level console: 0 or 1'),
  ],
  providers: [ApstoryLoggerService],
  bootstrap: [AppComponent]
})
export class AppModule { }

```

## Contact

Please contact Apstory on apstoryza@gmail.com if you have any questions.

## Microsoft Application Insights JavaScript SDK - Web

https://www.npmjs.com/package/@microsoft/applicationinsights-web


