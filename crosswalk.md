<table>
<thead>
  <tr>
    <th> FAIR principle </th>
    <th> How the SPARC guidelines adhere to the FAIR principle </th>
  </tr>
</thead>

<tbody>

<tr>
<td>F1: (Meta) data are assigned globally unique and persistent identifiers</td>
<td>Research data published on the Pennsieve platform are assigned a DOI through DataCite. DOIs are unique (randomly generated strings consisting of numbers and letters) identifiers that are permanently linked to published data.</td>
</tr>

<tr>
<td>F2: Data are described with rich metadata</td>
<td>The SDS (SPARC Dataset Structure) mandates several metadata files to be included along with research data. The required metadata acts to both describe high level information describing the dataset and rich metadata such as the Subjects file which contain information about the subjects research data was derived from, as well as manifest files which describe the structure of the dataset.</td>
</tr>

<tr>
<td>F3: Metadata clearly and explicitly include the identifier of the data they describe</td>
<td>The SPARC guidelines do not explicitly require the identifier to be embedded in the data. DOIs are generated via DataCite, however, this is only linked digitally apart from the research data.</td>
</tr>

<tr>
<td>F4: (Meta)data are registered or indexed in a searchable resource</td>
<td>Published research data is uploaded to Pennsieve Discover. Pennsieve discover provides both a web platform that allows individuals to view and download data, as well as an API which allows machines to access and analyze SPARC data.</td>
</tr>

<tr>
<td>A1: (Meta)data are retrievable by their identifier using a standardised communication protocol</td>
<td>Pennsieve provides an HTTP endpoint that allows for Pennsieve dataset IDs to be retrieved. Once the datataset ID is obtained, The Pennsiee ZipIt service can be accessed over HTTP to retrieve the data.</td>
</tr>

<tr>
<td>A1.1: The protocol is open, free and universally implementable</td>
<td>The Pennsieve API is open, free, and universally implementable</td>
</tr>

<tr>
<td>A1.2: The protocol allows for an authentication and authorization procedure where necessary</td>
<td>SPARC datasets posted on Pennsieve have two levels of authentication/authorization for data being accessed via their web platform or API: organizational level authorization as well as individual user authorization. Organization authorization ensures only members of our organization can access data. Individual user authorization ensures only individuals that you have explicitly given the appropriate permissions to can view the data. Once data is published, the authorization requirements are removed allowing anyone to consume the data.</td>
</tr>

<tr>
<td>A2: Metadata should be accessible even when the data is no longer available</td>
<td>SPARC data submitted to the SPARC portal is highly accessible for a minimum of 10 years, or longer if additional funding for hosting the data is provisioned. After the dataset is deprecated, the DOI can continue to be used to retrieve the dataset's metadata.</td>
</tr>

<tr>
<td>I1: (Meta)data use a formal, accessible, shared, and broadly applicable language for knowledge representation</td>
<td>SPARC data is formatted using the SPARC dataset structure, which is accessible to everyone on the SPARC portal. The metadata required by the SPARC data structure references data using Excel files, making it easily interpretable by human consumers of the data and suitable for machine learning or computational analysis.</td>
</tr>

<tr>
<td>I2: (Meta)data use vocabularies that follow the FAIR principles</td>
<td>SPARC provides a vocabulary term list that users can use to populate metadata using standard terminologies. The SPARC term list helps make datasets FAIR by:

1. Findability: The SPARC term list allows both humans and machines searching for SPARC terms over a span of datasets can more easily find their desired data.
2. Interoperability: The SPARC term list allows similar research datasets with matching standard terminologies to be merged to increase the quantity of analyzable data.</td>
</tr>

<tr>
<td>I3: (Meta)data include qualified references to other (meta)data</td>
<td>The SDS includes two metadata files that reference a dataset to other datasets:
1. The dataset_description metadata file: The description metadata file includes metadata that links to other related data via an identifier description, along with the fields relation type, identifier, and identifier type.
2. The subjects metadata file: The subjects metadata file includes a metadata field that allows you to link individual subjects to be linked to other datasets via the 'Also in dataset' field.</td>
</tr>

<tr>
<td>R1: (Meta)data are richly described with a plurality of accurate and relevant attributes</td>
<td>SPARC requires a multitude of metadata files that correspond to the structure of your data as well as the high level descrpition of it used to give the viewer a overview of the structure of the data.</td>
</tr>

<tr>
<td>R1.1: (Meta)data are released with a clear and accessible data usage license</td>
<td>While the SPARC does not specify that a license is to be explicitly included in SPARC metadata, licenses are able to be applied to SPARC's data repository Pennsieve.</td>
</tr>

<tr>
<td>R1.2: (Meta)data are associated with detailed provenance</td>
<td>SPARC requires two metadata files that provide provenance for the dataset:

1. The CHANGES metadata file: The CHANGES metadata file contains a list of changes made to the dataset since it's initial creation.
2. The dataset_description metadata file: the dataset_description provides a list of contributors that contributed to the generation of the data.</td>
</tr>

<tr>
<td>
R1.3: (Meta)data meet domain-relevant community standards
</td>
<td>The SPARC data platform provides a data standard for both research and computational data domains. Research data generally contains data derived from individual subjects (and samples derived from subjects), and the primary, source, and derivative folders allow raw and processed data to be separated and easily consumed by humans given the clear differentiation between the file types using high level folders. The code high level folder is available for computational code, as well as the code_description file which describes the code used for computational datasets.</td>
</tr>
