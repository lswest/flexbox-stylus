# flexbox-stylus

### A stylus library containing functions for generating flexbox prefixes.

## Usage

Just place the **flexbox.styl** file into your project, then import it in your stylus file with `@import 'flexbox'`  Each function tries to accept as many official values (according to the Flexbox standard), but does require some changes.

## Browser Support

Browser support can be seen here: http://caniuse.com/#search=flex-box

## Functions

- [`flexbox(value)`][flexbox] where value is either *flex*, or *inline-flex*.
- [`flex(value)`][flex] value represent the setting of basis, grow and shrink, example: `flex(25% 1 1)`
- [`flex-basis(value)`][flex-basis]
- [`flex-grow(value)`][flex-grow]
- [`flex-shrink(value)`][flex-shrink]
- [`flex-direction(value)`][flex-direction]`value` can be: *row*, *row-reverse*, *column* or *column-reverse*
- [`flex-wrap(value)`][flex-wrap] Accepts the 3 options: *nowrap*, *wrap*, *wrap-reverse*
- [`justify-content(value)`][justify-content] `value` can be: *start*, *end*, *center*, *space-bottom* or *space-around*
- [`align-content(value)`][align-content] `value` can be the same options as for `justify-content(value)`
- [`align-items(value)`][align-items] `value` can be: *start*, *end*, *stretch*, *center*, *baseline*
- [`align-self(value)`][align-self] accepts *start*, *end*, *auto*, *center*, *baseline*, *stretch*
- [`order(value)`][order] accepts any positive number

## Support

This code supports the following browsers:

Spec | Prefixed | Tweener
-----|----------|---------
Opera 12.1+ | Safari 6.1+ | IE 10
Chrome 29+ | iOS 7.1+ |
Firefox 28+ (current - 1) | |
Android Browser 4.4+ | |
IE 11+ | |

### Known bugs for IE 10 and 11

Ref: https://connect.microsoft.com/IE/feedback/details/802625/min-height-and-flexbox-flex-direction-column-dont-work-together-in-ie-10-11-preview

[flexbox]: https://developer.mozilla.org/en-US/docs/Web/Guide/CSS/Flexible_boxes
[flex]: https://developer.mozilla.org/en-US/docs/Web/CSS/flex
[flex-basis]: https://developer.mozilla.org/en-US/docs/Web/CSS/flex-basis
[flex-grow]: https://developer.mozilla.org/en-US/docs/Web/CSS/flex-grow
[flex-shrink]: https://developer.mozilla.org/en-US/docs/Web/CSS/flex-shrink
[flex-direction]: https://developer.mozilla.org/en-US/docs/Web/CSS/flex-direction
[flex-wrap]: https://developer.mozilla.org/en-US/docs/Web/CSS/flex-wrap
[justify-content]: https://developer.mozilla.org/en-US/docs/Web/CSS/justify-content
[align-content]: https://developer.mozilla.org/en-US/docs/Web/CSS/align-content
[align-items]: https://developer.mozilla.org/en-US/docs/Web/CSS/align-items
[align-self]: https://developer.mozilla.org/en-US/docs/Web/CSS/align-self
[order]: https://developer.mozilla.org/en-US/docs/Web/CSS/order