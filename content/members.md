<style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        #map {
            width: 100%;
            height: 600px;
            position: relative;
        }
        .point {
            fill: red;
            stroke: black;
            stroke-width: 1px;
            opacity: 0.8;
        }
</style>

# Members

NuGrid is an open, flexible collaboration involving researchers from
institutions from UK, USA, Canada, Italy, Switzerland, Spain, Portugal,
Germany, Hungary, Finland, China and Australia.
The collaboration is guided by the [Manifesto](manifesto.md), which defines the
collaboration rules.

### Principal Investigators

[Umberto Battino](mailto:umberto.battino@inaf.it)  
[Alison Laird](mailto:alison.laird@york.ac.uk)  
[Marco Pignatari](mailto:mpignatari@gmail.com)  
[Thanassis Psaltis](mailto:psaltis.tha@duke.edu)  
[Pavel Denissenkov](mailto:pavelden@uvic.ca)

### Points of contact

|Project coordinator | [Marco Pignatari](mailto:mpignatari@gmail.com) |
|Membership administrator| [Artemis Tsantiri](mailto:artemis.tsantiri@uregina.ca) |

### Members

|                                           Institute | Members                                  |
|----------------------------------------------------:|:-----------------------------------------|
|                            **Keele University, UK** | Raphael Hirschi (also Kavli IPMU, Japan) |
|                                                     | Etienne Kaiser                           |
|                                                     | Vishnu Varma                             |
|                      **University of Victoria, CA** | Falk Herwig                              |
|                                                     | Pavel Denisenkov                         |
|                                                     | Praneet Pathak                           |
|                                                     | Mallory Loria                            |
|                                                     | Joshua Issa                              |
|                                                     | Maeve Cockshutt                          |
|             **Los Alamos National Laboratory, USA** | Chris Fryer                              |
|                                                     | Rene Reifarth                            |
|                                                     | Andrés Yagüe López                       |
|                                                     | Samuel Jones                             |
|                                                     | Wes Even                                 |
|                                                     | Aaron Couture                            |
|                                                     | Stephen Andrews                          |
|                                                     | Mark Alexander Kaltenborn                |
|              **Observatory of Torino, INAF, Italy** | Claudia Travaglio                        |
|                          **University of Hull, UK** | Thomas Lawson                            |
|                                                     | James Keegans                            |
|                                                     | Thomas Trueman                           |
|                                                     | Paul Fong                                |
|                                                     | Kate Womack                              |
|                   **Arizona State University, USA** | Frank Timmes                             |
|                                                     | Morgan Taylor                            |
|                                                     | Ebraheem Farag                           |
|           **Goethe-Universität Frankfurt, Germany** | Kathrin Göbel                            |
|                                                     | Deniz Kurtulgil                          |
|                                      **TRIUMF, CA** | Chris Ruiz                               |
|                                                     | Barry Davids                             |
|                                                     | Alex Wen                                 |
|                     **Monash University, Australa** | Alexander Heger                          |
|                                                     | James Grimmett                           |
|                  **Michigan State University, USA** | Hendrik Schatz                           |
|                          **University of York, UK** | Alison Laird                             |
|                                                     | Sophie Abrahams                          |
|                                                     | Alexander Hall-Smith                     |
|                                                     | Lewis Todd                               |
|                                                     | May Haddaj Alruwaili                     |
|               **Oak Ridge Nationa Laboratory, USA** | Michael Bertolli                         |
| **Argonne National Laboatory, TechTrans Int., USA** | Benoit Côté                              |
|                      **University of Alabama, USA** | Dean Townsley                            |
|                           **SUNY Stony Brook, USA** | Alan Calder                              |
|              **CSIC-University of Valencia, Spain** | Cesar Domingo-Pardo                      |
|                                                     | Victor Babiano-Suarez                    |
|                                                     | Javier Balibrea Correa                   |
|                                                     | Jorge Lerendegui                         |
|                            **UPC-Barcelona, Spain** | Adria Casanovas-Hoste                    |
|                        **Brandeis University, USA** | Hungkwan Fok                             |
|                     **University of Edinburgh, UK** | Claudia Lederer-Woods                    |
|                                                     | Wan Aishah Wan Harun                     |
|                                                     | Ashley Tattersall                        |
|                                                     | Samuel Lloyd                             |
|                    **Konkoly Observatory, Hungary** | Marco Pignatari                          |
|              **Chinese Academy of Sciences, China** | Suqing Hou                               |
|                     **McMaster University, Canada** | Alan Chen                                |
|            **MPI for Intelligent Systems, Germany** | Jean-Claude Passy                        |
|             **Brookhaven National Laboratory, USA** | Shuya Ota                                |
|                                                     | Allyson Dewey                            |
|                   **University of Rijeka, Croatia** | Marina Manganaro                         |
|                                                     | Luka Božić                               |
|                                                     | Agata Vujić                              |
|                   **St. Mary's University, Canada** | Amanda Edwin                             |
|                **University of Jyväskylä, Finland** | Anu Kankainen                            |
|                               **EPFL, Switzerland** | Reto Trappitsch                          |
|                 **Saint Mary's University, Canada** | Thanassis Psaltis                        |
|                        **University of Surrey, UK** | Natalie Rees                             |
|                  **University of Lisbon, Portugal** | Margarida Paulino                        |
|                                                     | Daniel Galaviz                           |
|                                                     | Joao Afonso                              |
|     **Universita` di Napoli "Federico II", Italy**  | Umberto Battino                          |
| **INFN - Laboratori Nazionali del Sud (LNS), Italy**| Lorenzo Roberti                          |
|    **University of California, Berkeley, USA**      | Luca Boccioli                            |
|    **Heidelberg Institute for Theoretical Studies, Germany**      | Alexander Holas            |
|                  **University of Regina, Canada**   | Artemis Tsantiri                         |




World Map of the Collaboration
---

<div id="map"></div>

<script src="https://d3js.org/d3.v7.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/topojson@3"></script>
<script>

// Set the percentage of the screen the map will occupy
var mapWidthPercentage = 1;  // 100% of the parent width
var aspectRatio = 3 / 2;     // Aspect ratio (width:height)

// Define a projection and path generator
var projection = d3.geoMercator();
var path = d3.geoPath().projection(projection);

// Function to update the map size based on the container's width
function updateMapSize() {
    // Get the current width of the container (parent of #map)
    var width = document.getElementById('map').offsetWidth * mapWidthPercentage;

    // Calculate height based on the aspect ratio (3:2)
    var height = width / aspectRatio;

    // Update the SVG container with new width and height
    d3.select("svg")
        .attr("width", width)
        .attr("height", height);

    // Set a projection scale that ensures the map fits within the available space
    var scale = Math.min(width / 2, height / 2);  // Use half of the width or height to ensure map fits
    projection.scale(scale)
              .translate([width / 2, height / 1.5]); // Keep the center of the map

    // Redraw the map paths and points
    d3.selectAll("path").attr("d", path);
    d3.selectAll(".point")
        .attr("cx", function(d) { return projection([d.longitude, d.latitude])[0]; })
        .attr("cy", function(d) { return projection([d.longitude, d.latitude])[1]; });
}

// Create the SVG container for the map
var svg = d3.select("#map").append("svg");

// Load the world map data (TopoJSON)
d3.json("https://cdn.jsdelivr.net/npm/world-atlas@2/countries-50m.json").then(function(world) {

    // Draw the map using the data with grey color scheme
    svg.append("g")
        .selectAll("path")
        .data(topojson.feature(world, world.objects.countries).features)
        .enter().append("path")
        .attr("d", path)
        .attr("class", "country")
        .attr("fill", "#BEBEBE")  // Set the fill color to grey
        .attr("stroke", "#FFFFFF") // White borders for the countries
        .attr("stroke-width", 0.5);

    // Load the collaborators data from collaborators.json
    d3.json("https://nugrid.github.io/files/collaborators.json").then(function(collaborators) {

        // Plot the points for each collaborator
        svg.selectAll(".point")
            .data(collaborators)
            .enter().append("circle")
            .attr("class", "point")
            .attr("cx", function(d) { return projection([d.longitude, d.latitude])[0]; })
            .attr("cy", function(d) { return projection([d.longitude, d.latitude])[1]; })
            .attr("r", 5)
            .attr("title", function(d) { return d.name + " (" + d.city + ")"; });

    });

    // Initial map size update
    updateMapSize();

    // Listen for window resize events and update map size accordingly
    window.addEventListener('resize', updateMapSize);

    // Add drag behavior to allow map movement
    var drag = d3.drag()
        .on("drag", function(event) {
            var dx = event.dx;
            var dy = event.dy;

            // Translate projection based on drag distance
            var newTranslate = projection.translate();
            projection.translate([newTranslate[0] + dx, newTranslate[1] + dy]);

            // Redraw the map paths and points
            d3.selectAll("path").attr("d", path);
            d3.selectAll(".point")
                .attr("cx", function(d) { return projection([d.longitude, d.latitude])[0]; })
                .attr("cy", function(d) { return projection([d.longitude, d.latitude])[1]; });
        });

    // Apply drag behavior to the SVG container
    svg.call(drag);

});

</script>


Past members
---

**E.A. Milne Centre for Astrophysics, University of Hull, UK**: Jacob Brazier, Katherine Hall, Jasmine Stainton, Emilio Cuandu, Callum Silk, Meredith Sheppard, Adam Cox, William Bruce, Benjamin Brooks, Jacob Tomassi, William Logan, George Harvey, Stephane Trouille, William Wrathall, Richard Stancliffe, Jordan Schofield  

**University of Victoria, Canada**: Luke Siemens, John McKay, Christian Ritter, David Stephens, Ondrea Clarkson, Adam Paul

**University of York, UK**:Joscelyn Riley, Nic Hubbard, Chloe McElvaney, Josh Duncan, Emma Bendall, Ben Griffiths, Lewis Jones, Ben Shaw

**Universtaet Frankfurt, GSI, Germany**: Thien Tam Ngyuen, Paula Hillmann, Alexander Koloczek, Benedikt Thomas, Tanja Heftrich,Tanja Kausch, Rene Schach, Christoph Köppchen

**University of Sevilla, Institut de Fisica Corpuscolar of Valencia, Spain**: Pablo Gramage Iglesias, Carlos Guerrero, Jorge Lerendegui Marc

**Basel University, Switzerland**: Isabelle van Rijs

**Arizona State University, USA**: Eric Deleeuw, P. A. Young, Ilka Petermann

**Michigan State University, USA**: Ulrike Hager, Richard Cyburt, Carl Fields

**The Australian National University, Australia**: Aaron Dotter

**Louisiana State Universtiy USA**: Geoff Clayton, Kundam Kadam, Ischelle Martin

**University of Notre Dame, USA**: Mary Beard, Kiana Setoodehnia, Georgios Magkotsios

**Keele University, UK**: Nobuya Nishimura, C. Georgy, A. Kozyreva, M. Bennett

**Observatory of Torino, INAF, Italy**: S. Bisterzo

**Monash University, Australia**:Athira Menon

**University of Alabama, USA**:Broxton Miles

**TU Darmstadt, Germany**:Heiko Möller

**University of Chicago, USA**: Jim Truran, Claudio Ugalde

**TU Munich, Germany**: Shawn Bishop

**San Diego State University, USA**: Calvin Johnson

**Konkoly Observatory, Hungary**: Jacqueline den Hartogh
