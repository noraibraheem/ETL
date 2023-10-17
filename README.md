# ETL

<img src="https://github.com/noraibraheem/ETL/assets/62545277/6e836ce1-2dc6-4602-9aba-d9948d868605" alt="Image Description">


<h2>Extract</h2>
<p> extract process means gathering data from various sources, such as databases, files, APIs, or other data storage systems.In the context of the provided Python code, the "Extract" phase involves extracting data from CSV, JSON, and XML files using the respective functions <b></b>extract_from_csv</b>, <b>extract_from_json</b>, and <b>extract_from_xml</b>. These functions read the data from the files and return it as a pandas DataFrame. </p>

<p>The data from each source is accumulated into a single DataFrame named extracted_data which is later used in the transformation phase.
  
During the extraction process, any errors encountered during the data extraction are logged in the log file using the <b> log_progress function</b>, allowing you to monitor and debug any issues that may arise during the extraction phase.</p>

<p>The extracted data is then passed to the next phase, the "Transform" phase, where the data is processed and modified according to the defined transformation logic.</p>

<h2>Transform </h2>
<ls>Transforming data:
<li>standralization data formats and units of measurements</li>
<li>removing duplicates data</li>
<li>filtering out daat that's not required</li>
<li>establishing key relationships across tables</li>
</ls>

<h2> Load </h2>
<p> the <b>"Load"</b> phase involves the final step of the process where the transformed data is loaded into a target data repository, typically a <b>database</b>, a <b>data warehouse</b>, or a<b>data lake</b> . The main goal of the load phase is to make the processed data available for various types of analysis, reporting, or other downstream processes.</p>

<p>In the provided Python code, the <b>load_data</b> function is responsible for saving the transformed data into a CSV file. It utilizes the <b> to_csv</b> function from the pandas library to write the DataFrame to a CSV file. However, it's worth noting that in practice, the "Load" phase might involve loading data into a database or a data warehouse instead of just saving it to a CSV file.</p>
