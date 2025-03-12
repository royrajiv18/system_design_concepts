### a11y

## Assistive technology

- Keyboard only
- Screen reader
- mouse and pointer devices
- touchscreen gestures
- screen magnifiers

## Accessibility Standards -

WCAG (Web Content Accessibility Guideline) -

- Level A, Level AA, Level AAA

- WebAIM (WCAG Principles)
- Perceivable
- Operable
- Understandable
- Robust

## Screen reader

- Windows(Ctrl + Windows Key + Enter)
- Mac(cmd + f5)
- use semantic elements
- aria-hidden="true" or alt="" are similar
- Audio/Video - use transcript, captions
- use css class hidden in specific cases

### ARIA (Accessible Rich Internet Applications)

- Form: Labels
- aria-label
- aria-labelledBy
- aria-describedBy
- Todo - learn more about uses, role

### tabindex

- tabindex = "0" (follow the default order)
- tabindex = "1,2,3" (follow this order)
- tabindex = "-1" (skip from tab)

## Tab trapping - focus should always be in the modal if it is open

- logic:

  - if(isTabPressed){
    if(document.activeElement === modal){
    modal.focus()
    }

            if(document.activeElement === lastFocusableElement){
                modal.focus()
            }

    }

## contrast - open dev tool, select text and see contrast in colour section

### a11y check points -

- use semantic html
- add label to form elements
- use contrasting colours
- write descriptive links
- keep pinch and zoom alive
- provide text for non text content
- show where yoor focus is
- understandable without colour (give error icon along with red text)
- caption audio and video
- use aria only if necessary
- avoid use body: focus {outline: none}
- avoid use tabindex = "-1"
- avoid use aria-hidden="true"

### test for accessibility

- zoom to 400%
- check keyboard navigation
- turn your monitor off and use screen reader
- run lighthouse accessibility audit
- deactivate css and check if document structur still make sense
