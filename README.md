# flexbox-stylus

### A stylus library containing functions for generating flexbox prefixes.

## Usage

Just place the **flexbox.styl** file into your project, then import it in your stylus file with `@import 'flexbox'`  Each function tries to accept as many official values (according to the Flexbox standard), but does require some changes.

## Functions

- `flexbox(value)` where value is either *flex*, or *inline-flex*.
- `flex(size, grow, shrink, basis)` Each value except *grow* is optional.  *Size* is used for a width attribute (for legacy browsers).  To only set the grow value, use `flex(grow: 1)`.  The same format can be used to set any specific arguments.
- `flex-direction(value)``value` can be: *row*, *row-reverse*, *column* or *column-reverse* - Function for Flexbox's **flex-direction**
- `flex-wrap(value)` Accepts the 3 options: *nowrap*, *wrap*, *wrap-reverse* - Function for Flexbox's **flex-wrap**
- `flex-justify(value)` `value` can be: *start*, *end*, *center*, *space-bottom* or *space-around* - Function for Flexbox's **justify-content**
- `flex-content(value)` `value` can be the same options as for `flex-justify(value)` - Function for Flexbox's **align-content**
- `flex-align(value)` `value` can be: *start*, *end*, *stretch*, *center*, *baseline* - Function for Flexbox's **align-items**
- `flex-self(value)` accepts *start*, *end*, *auto*, *center*, *baseline*, *stretch* - Function for Flexbox's **align-self**
- `flex-group(value)` accepts any positive number - Function for Flexbox's **order** attribute
- `flex-firefox()` Helper function for legacy Firefox (where Flexboxes were treated as inline items).  Place it inside the firefox-only selector (`@-moz-document url-prefix()`).  See the **example.styl** file for an example.
