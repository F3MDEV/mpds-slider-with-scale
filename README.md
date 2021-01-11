<p align="center">
  <a href="https://mpds.f3m.pt/" rel="noopener" target="_blank"><img width="350" src="https://i.imgur.com/OANOfLI.png" alt="MPDS logo"></a></p>
</p>

<h1 align="center">MpDS Slider-With-Scale</h1>

<div align="center">

[React](https://reactjs.org/) component for faster and simpler web development.
<!--
[![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/mui-org/material-ui/blob/master/LICENSE)
[![npm latest package](https://img.shields.io/npm/v/@material-ui/core/latest.svg)](https://www.npmjs.com/package/@material-ui/core)
[![npm next package](https://img.shields.io/npm/v/@material-ui/core/next.svg)](https://www.npmjs.com/package/@material-ui/core)
[![npm downloads](https://img.shields.io/npm/dm/@material-ui/core.svg)](https://www.npmjs.com/package/@material-ui/core)
[![CircleCI](https://img.shields.io/circleci/project/github/mui-org/material-ui/next.svg)](https://app.circleci.com/pipelines/github/mui-org/material-ui?branch=next)
[![Coverage Status](https://img.shields.io/codecov/c/github/mui-org/material-ui/next.svg)](https://codecov.io/gh/mui-org/material-ui/branch/next)
[![Follow on Twitter](https://img.shields.io/twitter/follow/MaterialUI.svg?label=follow+Material-UI)](https://twitter.com/MaterialUI)
[![Dependabot Status](https://api.dependabot.com/badges/status?host=github&repo=mui-org/material-ui)](https://dependabot.com)
[![Average time to resolve an issue](https://isitmaintained.com/badge/resolution/mui-org/material-ui.svg)](https://isitmaintained.com/project/mui-org/material-ui 'Average time to resolve an issue')
[![Crowdin](https://badges.crowdin.net/material-ui-docs/localized.svg)](https://translate.material-ui.com/project/material-ui-docs)
[![Open Collective backers and sponsors](https://img.shields.io/opencollective/all/material-ui)](https://opencollective.com/material-ui) -->

</div>

## Installation

MpDS Slider-With-Scale is available as an [npm package](npm i mpds-slider-with-scale).

```sh
// with npm
npm i mpds-slider-with-scale

```
## Usage

Here is a quick example to get you started, **it's all you need**:

```tsx
import * as React from "react";
import MpdsSliderWithScale from "mpds-slider-with-scale"

function App() {
  return <MpdsSliderWithScale backButtonDisable="true"></MpdsSliderWithScale>
}

ReactDOM.render(<App />, document.querySelector('#app'));
```

<h4>Props</h4>

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Description</th>
      <th>Default</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <span>ariaValueText</span>
      </td>
      <td>
        <div>
          <span>A string value that provides a user-friendly name for the current value of the slider.</span>
        </div>
        <div>
          <div>
            <span>any</span>
          </div>
        </div>
      </td>
      <td>
        <span>-</span>
      </td>
    </tr>
    <tr>
      <td>
        <span>getAriaLabel</span>
      </td>
      <td>
        <div>
          <span>Accepts a function which returns a string value that provides a user-friendly name for the thumb labels of the slider.</span>
        </div>
        <div>
          <div>
            <span>any</span>
          </div>
        </div>
      </td>
      <td>
        <span>-</span>
      </td>
    </tr>
    <tr>
      <td>
        <span>ariaLabelledby</span>
      </td>
      <td>
        <div>
          <span>The id of the element containing a label for the slider.</span>
        </div>
        <div>
          <div>
            <span>string</span>
          </div>
        </div>
      </td>
      <td>
        <span>-</span>
      </td>
    </tr>
    <tr>
      <td>
        <span>ariaLabel</span>
      </td>
      <td>
        <div>
          <span>The label of the slider.</span>
        </div>
        <div>
          <div>
            <span>string</span>
          </div>
        </div>
      </td>
      <td>
        <span>-</span>
      </td>
    </tr>
    <tr>
      <td>
        <span>initialValue</span>
      </td>
      <td>
        <div>
          <span>The default element value. Use when the component is not controlled.</span>
        </div>
        <div>
          <span>number | number[]</span>
        </div>
      </td>
      <td>
        <span>-</span>
      </td>
    </tr>
    <tr>
      <td>
        <span>numberOfStepsPerMove</span>
      </td>
      <td>
        <div>
          <p>The granularity with which the slider can step through values. (A "discrete" slider.) The min prop serves as the origin for the valid values. We recommend (max - min) to be evenly divisible by the step.
When step is null, the thumb can only be slid onto marks provided with the marks prop.</p>
        </div>
        <div>
          <div>
            <span>number</span>
          </div>
        </div>
      </td>
      <td>
        <span>-</span>
      </td>
    </tr>
    <tr>
      <td>
        <span>marksLabels</span>
      </td>
      <td>
        <div>
          <span>Marks indicate predetermined values to which the user can move the slider. If true the marks will be spaced according the value of the step prop. If an array, it should contain objects with value and an optional label keys.</span>
        </div>
        <div>
          <span>boolean | any[]</span>
        </div>
      </td>
      <td>
        <span>-</span>
      </td>
    </tr>
    <tr>
      <td>
        <span>minNumber</span>
      </td>
      <td>
        <div>
          <span>The minimum allowed value of the slider. Should not be equal to max.</span>
        </div>
        <div>
          <div>
            <span>number</span>
          </div>
        </div>
      </td>
      <td>
        <span>-</span>
      </td>
    </tr>
    <tr>
      <td>
        <span>maxNumber</span>
      </td>
      <td>
        <div>
          <span>The maximum allowed value of the slider. Should not be equal to min.</span>
        </div>
        <div>
          <div>
            <span>number</span>
          </div>
        </div>
      </td>
      <td>
        <span>-</span>
      </td>
    </tr>
    <tr>
      <td>
        <span>thumbHTMLElement</span>
      </td>
      <td>
        <div>
          <span>The component used to display the value label.</span>
        </div>
        <div>
          <div>
            <span>any</span>
          </div>
        </div>
      </td>
      <td>
        <span>-</span>
      </td>
    </tr>
    <tr>
      <td>
        <span>displayValueBallon</span>
      </td>
      <td>
        <div>
          <p>Controls when the value label is displayed: - auto the value label will display when the thumb is hovered or focused. - on will display persistently. - off will never display.</p>
        </div>
        <div>
          <div>
            <span>any</span>
          </div>
        </div>
      </td>
      <td>
        <span>-</span>
      </td>
    </tr>
    <tr>
      <td>
        <span>labelFormat</span>
      </td>
      <td>
        <div>
          <p>The format function the value label's value. When a function is provided, it should have the following signature: - {number} value The value label's value to format - {number} index The value label's index to format</p>
        </div>
        <div>
          <div>
            <span>any</span>
          </div>
        </div>
      </td>
      <td>
        <span>-</span>
      </td>
    </tr>
    <tr>
      <td>
        <span>disabled</span>
      </td>
      <td>
        <div>
          <span>If true, the slider will be disabled.</span>
        </div>
        <div>
          <div>
            <span>boolean</span>
          </div>
        </div>
      </td>
      <td>
        <span>-</span>
      </td>
    </tr>
    <tr>
      <td>
        <span>barProps</span>
      </td>
      <td>
        <div>
          <span>Checks if the button should be disabled</span>
        </div>
        <div>
          <div>
            <span>string</span>
          </div>
        </div>
      </td>
      <td>
        <span>-</span>
      </td>
    </tr>
    <tr>
      <td>
        <span>name</span>
      </td>
      <td>
        <div>
          <span>Name attribute of the hidden input element.</span>
        </div>
        <div>
          <div>
            <span>string</span>
          </div>
        </div>
      </td>
      <td>
        <span>-</span>
      </td>
    </tr>
    <tr>
      <td>
        <span>widthOfTheSlide</span>
      </td>
      <td>
        <div>
          <span>Width of the slider</span>
        </div>
        <div>
          <div>
            <span>string</span>
            <span>number</span>
          </div>
        </div>
      </td>
      <td>
        <span>-</span>
      </td>
    </tr>
    <tr>
      <td>
        <span>valueSlider</span>
      </td>
      <td>
        <div>
          <span>Actual value of the slider</span>
        </div>
        <div>
          <div>
            <span>any</span>
          </div>
        </div>
      </td>
      <td>
        <span>-</span>
      </td>
    </tr>
    <tr>
      <td>
        <span>sliderMainColor</span>
      </td>
      <td>
        <div>
          <span>Color of the thumb</span>
        </div>
        <div>
          <div>
            <span>string</span>
          </div>
        </div>
      </td>
      <td>
        <div>
          <span>#06B9E4</span>
        </div>
      </td>
    </tr>
    <tr>
      <td>
        <span>arrowTooltipColor</span>
      </td>
      <td>
        <div>
          <span>Color of the arrow under the tooltip</span>
        </div>
        <div>
          <div>
            <span>String</span>
          </div>
        </div>
      </td>
      <td>
        <div>
          <span>#FBAF30</span>
        </div>
      </td>
    </tr>
    <tr>
      <td>
        <span>tooltipColor</span>
      </td>
      <td>
        <div>
          <span>Tooltip color element</span>
        </div>
        <div>
          <div>
            <span>String</span>
          </div>
        </div>
      </td>
      <td>
        <div>
          <span>#FBAF30</span>
        </div>
      </td>
    </tr>
    <tr>
      <td>
        <span>onChange</span>
      </td>
      <td>
        <div>
          <span>Callback function that is fired when the slider's value changed.</span>
        </div>
        <div>
          <span>((event: object, value: number | number[]) =&gt; void)</span>
        </div>
      </td>
      <td>
        <span>-</span>
      </td>
    </tr>
    <tr>
      <td>
        <span>firstScale</span>
      </td>
      <td>
        <div>
          <span>First scale text</span>
        </div>
        <div>
          <div>
            <span>String</span>
          </div>
        </div>
      </td>
      <td>
        <div>
          <span>Low</span>
        </div>
      </td>
    </tr>
    <tr>
      <td>
        <span>secondScale</span>
      </td>
      <td>
        <div>
          <span>Second scale text</span>
        </div>
        <div>
          <div>
            <span>String</span>
          </div>
        </div>
      </td>
      <td>
        <div>
          <span>Moderate</span>
        </div>
      </td>
    </tr>
    <tr>
      <td>
        <span>thirdScale</span>
      </td>
      <td>
        <div>
          <span>Third scale text</span>
        </div>
        <div>
          <div>
            <span>String</span>
          </div>
        </div>
      </td>
      <td>
        <div>
          <span>High</span>
        </div>
      </td>
    </tr>
  </tbody>
</table>
<br>
Yes, it's really all you need to get started! Try it in:
[CodeSandbox](https://codesandbox.io/)
<br>

## License

No License. "(...) nobody else can copy, distribute, or modify your work without being at risk of take-downs, shake-downs, or litigation."
