---
title       : Dynamische Datenvisualisierung
subtitle    : Proof of Concept
author      : Christian Kamenik
job         : Projektleiter Verknüpfte Auswertungen
logo        : Logo_V_ADMAS_small.png
biglogo     : Logo_V_ADMAS.png
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [bootstrap]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
---








## Stand Medienmitteilung 2013

[MM2013](http://www.astra.admin.ch/dokumentation/00109/00113/00491/index.html?lang=de&print_style=yes&msg-id=47737)

---

## Stand Business Objects

![alt text](assets/img/Unbenannt-1.png)

---

## Stand Business Objects

![alt text](assets/img/Unbenannt-3.png)

---

## Stand dynamische Datenvisualisierung

#### Gründe für Führerausweisentzüge im Jahr 2012  

<!-- PieChart generated in R 2.15.1 by googleVis 0.4.5 package -->
<!-- Tue Nov 19 21:24:30 2013 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataPieChartIDf9e1b2eb755 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
 "Missachten von Geschwindigkeitsvorschriften",
30646 
],
[
 "Angetrunkenheit (>=0,80 ‰)",
16768 
],
[
 "Unaufmerksamtkeit",
9385 
],
[
 "Missachten des Vortritts",
4081 
],
[
 "Nichtbeachten von Signalen",
1472 
],
[
 "Unzulässiges Überholen",
1789 
],
[
 "Andere Fahrfehler",
4702 
],
[
 "Trunksucht",
1701 
],
[
 "Einfluss von Medikamenten oder Drogen",
2771 
],
[
 "Drogensucht",
2409 
],
[
 "Krankheit oder Gebrechen",
4174 
],
[
 "Übrige Gründe",
20284 
] 
];
data.addColumn('string','Y.NA');
data.addColumn('number','Y.2012');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartPieChartIDf9e1b2eb755() {
var data = gvisDataPieChartIDf9e1b2eb755();
var options = {};
options["allowHtml"] = true;
options["width"] =   1000;
options["height"] =    450;
options["pieHole"] =    0.4;
options["pieResidueSliceLabel"] = "Rest";
options["pieSliceText"] = "none";
options["chartArea"] = {left:0,top:100,width:900,height:300};
options["legend"] = {position: 'right'};

    var chart = new google.visualization.PieChart(
    document.getElementById('PieChartIDf9e1b2eb755')
    );
    chart.draw(data,options);
    

}
  
 
// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "corechart";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartPieChartIDf9e1b2eb755);
})();
function displayChartPieChartIDf9e1b2eb755() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}
 
// jsFooter
</script>
 
<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartPieChartIDf9e1b2eb755"></script>
 
<!-- divChart -->
  
<div id="PieChartIDf9e1b2eb755"
  style="width: 1000px; height: 450px;">
</div>


---

## Stand dynamische Datenvisualisierung

#### Anzahl der Führerausweisentzüge nach Alter und Jahr

<iframe src=assets/fig/MultiBar.html seamless></iframe>


---

## Stand dynamische Datenvisualisierung

#### Massnahmen (Entzüge) gegenüber Motorfahrzeugführern

<!-- LineChart generated in R 2.15.1 by googleVis 0.4.5 package -->
<!-- Wed Nov 13 21:39:28 2013 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataLineChartID3a84608d5a5 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
 1986,
4833,
24421 
],
[
 1987,
305,
3395 
],
[
 1988,
428,
4677 
],
[
 1989,
442,
4336 
],
[
 1990,
476,
4408 
],
[
 1991,
535,
4785 
],
[
 1992,
631,
5800 
],
[
 1993,
634,
6626 
],
[
 1994,
571,
7191 
],
[
 1995,
542,
7387 
],
[
 1996,
614,
7693 
],
[
 1997,
602,
8731 
],
[
 1998,
689,
10011 
],
[
 1999,
739,
11080 
],
[
 2000,
907,
13428 
],
[
 2001,
1004,
17370 
],
[
 2002,
1348,
25633 
],
[
 2003,
1350,
26309 
],
[
 2004,
1311,
31744 
],
[
 2005,
1400,
32933 
],
[
 2006,
1818,
44123 
],
[
 2007,
2561,
68358 
],
[
 2008,
2585,
69693 
],
[
 2009,
2758,
72459 
],
[
 2010,
2858,
76212 
],
[
 2011,
2739,
74057 
],
[
 2012,
3060,
75206 
],
[
 2013,
2688,
66989 
] 
];
data.addColumn('number','Zeit');
data.addColumn('number','Entzug des Lernfahrausweises');
data.addColumn('number','Entzug des Führerausweises');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartLineChartID3a84608d5a5() {
var data = gvisDataLineChartID3a84608d5a5();
var options = {};
options["allowHtml"] = true;
options["width"] =   1000;
options["height"] =    500;
options["chartArea"] = {left:0,top:50,width:600,height:300};

    chartLineChartID3a84608d5a5 = new google.visualization.ChartWrapper({
    dataTable: data,       
    chartType: 'LineChart',
    containerId: 'LineChartID3a84608d5a5',
    options: options
    });
    chartLineChartID3a84608d5a5.draw();
    

}

  function openEditorLineChartID3a84608d5a5() {
  var editor = new google.visualization.ChartEditor();
  google.visualization.events.addListener(editor, 'ok',
  function() { 
  chartLineChartID3a84608d5a5 = editor.getChartWrapper();  
  chartLineChartID3a84608d5a5.draw(document.getElementById('LineChartID3a84608d5a5')); 
  }); 
  editor.openDialog(chartLineChartID3a84608d5a5);
  }
    
 
// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "charteditor";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartLineChartID3a84608d5a5);
})();
function displayChartLineChartID3a84608d5a5() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}
 
// jsFooter
</script>
 
<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartLineChartID3a84608d5a5"></script>
 
<!-- divChart -->
<input type='button' onclick='openEditorLineChartID3a84608d5a5()' value='Edit me!'/>  
<div id="LineChartID3a84608d5a5"
  style="width: 1000px; height: 500px;">
</div>


---

## Stand dynamische Medienmitteilung

[MM2014](http://www.astra.admin.ch/dokumentation/00109/00113/00491/index.html?lang=de&print_style=yes&msg-id=47737)
