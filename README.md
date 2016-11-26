# Wii-U-title-info-database
A Wii U title info database with title id, name, region, content type, online ticket availability, human readable size, and raw size in bytes.

The database has one table named "titles" and eight value fields: "title_id", "title_key", "name", "region", "content_type", "size", "raw_size", and "ticket".

Things to know:
 This is a sqlite database
 There is no value in the title_key field, it is left blank on purpose
 The "size" field is a human readable size for the title, if this value is 0 that means I couldn not download the tmd for that title.
 The "raw_size" field is the title size in bytes, if this value is 0 then I couldn not download the tmd
 The "ticket" field represents whether or not the title has an online ticket available on that key site. 0=False,1=True.
 I have exclued all titles without a name on that key site. As soon as a name is given to the title then I will include it in the database.

