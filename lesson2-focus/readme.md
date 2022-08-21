![](../../../../../var/folders/t2/0_b2q0890xx6bfmw229z263h0000gp/T/TemporaryItems/NSIRD_screencaptureui_qGHZ8b/Screenshot 2022-08-21 at 9.50.45 AM.png)
- https://html.spec.whatwg.org/multipage/interaction.html#the-tabindex-attribute
- The tabindex content attribute allows authors to make an element and regions that have the element as its DOM anchor
  be focusable areas, allow or prevent them from being sequentially focusable, and determine their relative ordering for
  sequential focus navigation.

- The name "tab index" comes from the common use of the Tab key to navigate through the focusable elements. The term "
  tabbing" refers to moving forward through sequentially focusable focusable areas.

- The tabindex attribute, if specified, must have a value that is a valid integer. Positive numbers specify the relative
  position of the element's focusable areas in the sequential focus navigation order, and negative numbers indicate that
  the control is not sequentially focusable.

- Developers should use caution when using values other than 0 or −1 for their tabindex attributes as this is
  complicated to do correctly.

- The following provides a non-normative summary of the behaviors of the possible tabindex attribute values. The below
  processing model gives the more precise rules.

omitted (or non-integer values)

- The user agent will decide whether the element is focusable, and if it is, whether it is sequentially focusable or
  click focusable (or both).
  −1 (or other negative integer values)
- Causes the element to be focusable, and indicates that the author would prefer the element to be click focusable but
  not sequentially focusable. The user agent might ignore this preference for click and sequential focusability, e.g.,
  for specific element types according to platform conventions, or for keyboard-only users.
  0

- Causes the element to be focusable, and indicates that the author would prefer the element to be both click focusable
  and sequentially focusable. The user agent might ignore this preference for click and sequential focusability.
  positive integer values
- Behaves the same as 0, but in addition creates a relative ordering within a tabindex-ordered focus navigation scope,
  so that elements with higher tabindex attribute value come later.
  Note that the tabindex attribute cannot be used to make an element non-focusable. The only way a page author can do
  that is by disabling the element, or making it inert.
- ![](../../../../../var/folders/t2/0_b2q0890xx6bfmw229z263h0000gp/T/TemporaryItems/NSIRD_screencaptureui_U5Zg6E/Screenshot 2022-08-21 at 10.08.23 AM.png)![](../../../../../var/folders/t2/0_b2q0890xx6bfmw229z263h0000gp/T/TemporaryItems/NSIRD_screencaptureui_ZaPrsN/Screenshot 2022-08-21 at 10.15.55 AM.png)![](../../../../../var/folders/t2/0_b2q0890xx6bfmw229z263h0000gp/T/TemporaryItems/NSIRD_screencaptureui_2ukzng/Screenshot 2022-08-21 at 10.22.24 AM.png)![](../../../../../var/folders/t2/0_b2q0890xx6bfmw229z263h0000gp/T/TemporaryItems/NSIRD_screencaptureui_7h54VV/Screenshot 2022-08-21 at 10.26.56 AM.png)![](../../../../../var/folders/t2/0_b2q0890xx6bfmw229z263h0000gp/T/TemporaryItems/NSIRD_screencaptureui_XoA4of/Screenshot 2022-08-21 at 10.33.39 AM.png)


use the html element so that we can native accessbilty 