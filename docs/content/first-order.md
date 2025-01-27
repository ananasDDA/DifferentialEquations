# First Order Differential Equations

## Linear First Order DEs

A linear first order differential equation has the form:

\\[ \frac{dy}{dx} + P(x)y = Q(x) \\]

The solution is given by the integrating factor method:

\\[ y = e^{-\int P(x)dx} \left( \int Q(x)e^{\int P(x)dx}dx + C \right) \\]

For inline equations, use: The slope is given by \\( \frac{dy}{dx} \\).

## Interactive Example

<div class="geogebra" id="ggb-element"></div>

<script src="https://www.geogebra.org/apps/deployggb.js"></script>
<script>
    var params = {
        "appName": "graphing",
        "width": 800,
        "height": 600,
        "showToolBar": false,
        "showAlgebraInput": false,
        "showMenuBar": false,
        "showResetIcon": true,
        "enableLabelDrags": false,
        "enableShiftDragZoom": true,
        "enableRightClick": false,
        "material_id": "YOUR_GEOGEBRA_ID"
    };
    var applet = new GGBApplet(params, true);
    window.addEventListener("load", function() {
        applet.inject('ggb-element');
    });
</script>