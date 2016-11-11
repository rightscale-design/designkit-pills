# Designkit Pills

## Install

```bash
npm i designkit-pills
```

## Usage

```html

<div class="simple_pill">
  <i></i>thumb pill
</div>

<div class="thumb_pill added remove">
  <i></i>thumb pill
</div>
```

## The CSS

```css
/*
//
// designkit-pills
// --------------------------------------------------
*/
.simple_pill, .thumb_pill {
  border-radius: 3px;
  border: 1px solid #D1D6DC;
  color: #76899A;
  display: table;
  font-size: 1.1rem;
  line-height: 1.7;
  padding: 0 1rem;
}

.thumb_pill {
  color: #76899A;
  padding-left: 0;
  position: relative;
}

.thumb_pill i {
  background-color: #D1D6DC;
  display: block;
  float: left;
  height: 1.8rem;
  margin-right: .6rem;
  overflow: hidden;
  width: 2.1rem;
}

.thumb_pill i:after, .thumb_pill i:before {
  content: '';
  position: absolute;
  width: inherit;
  height: inherit;
  top: 0;
  left: 0;
  background: no-repeat center center transparent;
  -webkit-transition: all 0.14s ease-in;
  -moz-transition: all 0.14s ease-in;
  transition: all 0.14s ease-in;
}

.thumb_pill i:before {
  top: -100%;
}

.thumb_pill i:after {
  background: url("generic_white.svg") no-repeat center center transparent;
  background-size: 1.5rem;
}

.thumb_pill.add:hover, .thumb_pill.remove:hover, .thumb_pill.reassign:hover {
  cursor: pointer;
  cursor: hand;
}

.thumb_pill.add:hover i:after, .thumb_pill.remove:hover i:after, .thumb_pill.reassign:hover i:after {
  top: 100%;
}

.thumb_pill.add:hover, .thumb_pill.add.checked {
  border-color: #0A83F6;
}

.thumb_pill.add:hover i, .thumb_pill.add.checked i {
  background-color: #0A83F6;
}

.thumb_pill.add:hover i:before, .thumb_pill.add.checked i:before {
  background: url("plus.svg") no-repeat center center transparent;
  background-size: 1.1rem;
  top: 0;
}

.thumb_pill.add:hover i:after, .thumb_pill.add.checked i:after {
  top: 100%;
}

.thumb_pill.added {
  border-color: #80C11A;
}

.thumb_pill.added i {
  background-color: #80C11A;
}

.thumb_pill.added i:after {
  background: url("generic_white.svg") no-repeat center center transparent;
  background-size: 1.5rem;
}

.thumb_pill.selected {
  border-color: #0A83F6;
}

.thumb_pill.selected i {
  background-color: #0A83F6;
}

.thumb_pill.selected i:before {
  background: url("generic_white.svg") no-repeat center center transparent;
  background-size: 1.5rem;
  top: 0;
}

.thumb_pill.selected i:after {
  background: none;
}

.thumb_pill.reassign:hover, .thumb_pill.reassign.checked {
  border-color: #0A83F6;
}

.thumb_pill.reassign:hover i, .thumb_pill.reassign.checked i {
  background-color: #0A83F6;
}

.thumb_pill.reassign:hover i:before, .thumb_pill.reassign.checked i:before {
  background: url("reassign_white.svg") no-repeat center center transparent;
  background-size: 1.1rem;
  top: 0;
}

.thumb_pill.reassign:hover i:after, .thumb_pill.reassign.checked i:after {
  top: 100%;
}

.thumb_pill.remove:hover, .thumb_pill.remove.checked {
  border-color: #C32525;
}

.thumb_pill.remove:hover i, .thumb_pill.remove.checked i {
  background-color: #C32525;
}

.thumb_pill.remove:hover i:before, .thumb_pill.remove.checked i:before {
  background: url("minus.svg") no-repeat center center transparent;
  background-size: 1.1rem;
  top: 0;
}

.thumb_pill.remove:hover i:after, .thumb_pill.remove.checked i:after {
  top: 100%;
}

.thumb_pill.w_checkbox {
  padding-right: 3rem;
  position: relative;
  display: -webkit-box;
  display: -moz-box;
  display: box;
  display: -webkit-flex;
  display: -moz-flex;
  display: -ms-flexbox;
  display: flex;
}

.thumb_pill.w_checkbox .checkbox_wrap {
  position: absolute;
  right: -.5rem;
  top: 50%;
}
```

## Author

Artur Janas

## License

The MIT License (MIT)

Copyright (c) 2016 RightScale

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
