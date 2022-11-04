# USA Names
This data comes form the Social Security Administration Names data.  The
data contains the number of births for each state, year and gender.

This data model is written in [Malloy](https://github.com/looker-open-source/malloy/).

[Source code for the model on Github](https://github.com/lloydtabb/name_fiddle/blob/main/names_composer.malloy)


## Names by Generation

See each generations most popular names and which states they are most popular in.

#### <!--malloy-query model="names_composer.malloy" source="names2" query="current_f"--> `Current Female Names` - Most popular female names on or after 2010

#### <!--malloy-query model="names_composer.malloy" source="names2" query="current_m"--> `Current Male Names` - Most popular male names on or after 2010

#### <!--malloy-query model="names_composer.malloy" source="names2" query="gen_z_f"--> `Gen Z Female Names` - Most popular female names between 1995 and 2010

#### <!--malloy-query model="names_composer.malloy" source="names2" query="gen_z_m"--> `Gen Z Male Names` - Most popular male names between 1995 and 2010

#### <!--malloy-query model="names_composer.malloy" source="names2" query="millenial_f"--> `Millenial Female Names` - Most popular female names between 1980 and 1996

#### <!--malloy-query model="names_composer.malloy" source="names2" query="millenial_m"--> `Millenial Male Names` - Most popular male names between 1980 and 1996


## Iconic Names

For each state, what are the most Iconic names (unusally popular)

#### <!--malloy-query model="names_composer.malloy" source="names2" query="iconic_names_by_state"--> `Iconic Names by State`
 
## Names and Gender
Some names are gender neutral or gender specific by time or region.  

#### <!--malloy-query model="names_composer.malloy" source="names2" query="gender_neutral_names"--> `Gender Neutral Name` - Some names can be are common for both female and male genders.  This query investigates gender neutral names and their use over time and location.

#### <!--malloy-query model="names_composer.malloy" source="names2" query="kelly_time_space_dashboard"--> `Kelly in Space and Time` - Examine the name 'Kelly' over time and location (in fine detail).  

## Resurgent Names
#### <!--malloy-query model="names_composer.malloy" source="names2" query="resurgent_names"--> `Resurgent Names` - Names, once popular, lose popularity and then, sometime later, re-gain popularity.  This query finds those names.  We find the two most popular decades for a given name and the time difference between them.

## About Composer

Composer is implemented using Malloy, DuckDB and WASM and runs completely
in your browser.  Javascript code is compled from here:

  https://github.com/malloydata/malloy-composer
  
 and distributed from here:
 
   https://github.com/lloydtabb/malloy_fiddle_dist
