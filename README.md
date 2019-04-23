# KharkivCSS
The Web Design Cheat Code: Using SVG to bridge CSS’ gaps - Lea Verou

Highly recommended book by Lea - https://www.amazon.com/CSS-Secrets-Lea-Verou/dp/1449372635?tag=leaverou-20

https://mavo.io/ - create webaps w/o backend

    svg viewbox attribute
        gives you coordinate system and direction
        defines aspect ratio
    data url usage allows inlining images, svg, html
        you can use <style> inside data url
        can be animated by keyframes
        → pactival appliance - rating widget on star emojis with fractional progress
        no string concatenation
        special parsing rules
        to reduce duplication - assign data-url to css variable
        you can use several backgrounds
    list-style-image
        with svg data
        cursor custom image - limited to 128px width-height
    implementing gradiend border
        svg inside <filter>
        <feTurbulence/> https://developer.mozilla.org/en-US/docs/Web/SVG/Element/feTurbulence
        https://developer.mozilla.org/en-US/docs/Web/SVG/Element/feDisplacementMap
        width & height can be done with calc
    squiggle vision demo


WCAG: accessibility in practice - Dmytro Popov

not really interesting talk about WCAG standarts


Logging productivity - Anton Nemtsev

https://github.com/SilentImp/performance

    measure concurents and making our product 20% better
    measurement types
        pipeline
        separate server
        RUM - real user measurements


CI:

    lighthouse metrics on gitlab
    server timing
        http headers
            serverTiming
            TrailerHeaders
            earlyHints (npm)
            clientHints
            Accept-CH (device-memory, DVR, Viewport-width, save-data, downlink) also available in navigator.connection
    Performance.Observable
        userTiming
        NavigationTiming
        resourceTiming
        expres-formidable - sendBeacon vs fetch


Houdini - Nikita Dubko

https://css-houdini.rocks/

pureCSS images

    CSS custom properties
    CSS parser API (window.CSSParseRule)
    Properties and values - registerProperty
    Worklets - separate thread w/o global scope
    CSS painting API (css qr code generator)
    Layout API
    Animation worklet
        scrolltimeline
        fontMetrics API (.measureElement)
        high performance
        easy to use


http://houdini.glitch.me/


Framer X - Valery Skorobohatko

demo presentation of Using Framer X


UX as a layout base - Olena Shpilevska

    UX is all about patterns
    devs to check designers
        Z-pattern and F-pattern
        axis of interaction
        ninjamock for wireframes
        https://whimsical.co/
    https://goodui.org/
    https://www.nngroup.com/articles/hamburger-menus/
    Dan Norman - Let'd not forget why we are here. Let's make products for people


WebFonts in 2019: Everything Changes - Chris Lilley


    variable fonts
    color fonts


Characters codepaint properties

glyph - visual representation of symbol

descriptors


Problem: using Latin glyphs in Japanese

    unicode range - descriptor for allowed range of unicode characters (U+26 == &)


Variable fonts

    design axis for fonts
    italic
    optical site
    slant angle
    width - condensity
    weight


    font-variation-settings
    font-optical-scaling

Color fonts

    emoji (first there were bitmaps for emojis -> then vectors)
    COLR+CPAL

CSS4- font palette

font-palette-value

    optional stylistic controls
    font-feature-settings
    font-variant-numeric
    diagonal fractions

https://wakamaifondue.com/