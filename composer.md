# USA Names
This data comes form the Social Security Administration Names data.  The
data contains the number of births for each state, year and gender.

Composer is implemented using Malloy, DuckDB and WASM and runs completely
in your browser.  Javascript code is compled from here:

  https://github.com/malloydata/malloy-composer
  
 and distributed from here:
 
   https://github.com/lloydtabb/malloy_fiddle_dist

# Queries for Malloy Composer

## Names by Generation

See each generations most popular names and which states they are most popular in.

#### <!--malloy-query model="names_composer.malloy" source="names2" query="current_f"--> `Current Female Names`

#### <!--malloy-query model="names_composer.malloy" source="names2" query="current_m"--> `Current Male Names`

#### <!--malloy-query model="names_composer.malloy" source="names2" query="gen_z_f"--> `Gen Z Female Names`

#### <!--malloy-query model="names_composer.malloy" source="names2" query="gen_z_m"--> `Gen Z Male Names`

#### <!--malloy-query model="names_composer.malloy" source="names2" query="millenial_f"--> `Millenial Female Names`

#### <!--malloy-query model="names_composer.malloy" source="names2" query="millenial_m"--> `Millenial Male Names`


## Iconic Names

For each state, what are the most Iconic names (unusally popular)

#### <!--malloy-query model="names_composer.malloy" source="names2" query="iconic_names_by_state"--> `Iconic Names by State`
 
## Names and Gender
Some names are gender neutral or gender specific by time or region.  

#### <!--malloy-query model="names_composer.malloy" source="names2" query="gender_neutral_names"--> `Gender Neutral Name`