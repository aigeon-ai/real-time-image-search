# Aigeon AI: Real-Time Image Search

## Project Description

Aigeon AI's Real-Time Image Search is a Python-based server application designed to provide users with the ability to perform real-time image searches across the web. This application leverages advanced search filters to refine image search results, making it a powerful tool for users who need precise and specific image data retrieval.

## Features Overview

- **Real-Time Image Search**: Perform searches for images across the web in real-time.
- **Advanced Filtering**: Utilize a wide range of filters to narrow down search results based on size, color, type, time, usage rights, file type, aspect ratio, country, and more.
- **Safe Search Options**: Control the display of explicit content in search results with safe search settings.
- **Region-Specific Searches**: Customize searches based on specific countries or regions.
- **Field Projection**: Specify which fields of image data to include in the response.

## Main Features and Functionality

1. **Search Images**: The core functionality of this application is to perform image searches using a variety of filters. Users can specify search queries and refine results based on multiple criteria, ensuring that the images returned meet their specific needs.

2. **Filter Options**: Users can apply filters such as:
   - **Size**: Filter images by size, ranging from icons to high-resolution images.
   - **Color**: Search for images with a dominant color.
   - **Type**: Specify the type of image, such as photos, clipart, or animated images.
   - **Time**: Limit results to images updated within a specific time frame.
   - **Usage Rights**: Filter images based on usage rights, such as creative commons or commercial use.
   - **File Type**: Specify the desired image format, including jpg, png, gif, etc.
   - **Aspect Ratio**: Search for images with specific aspect ratios, such as tall or panoramic.
   - **Country and Region**: Limit searches to images published in or queried from specific countries or regions.
   - **Safe Search**: Manage the display of explicit content in search results.

3. **Field Projection**: Users can choose to receive only specific fields of image data in the response, allowing for customized and efficient data retrieval.

## Main Functions Description

### `search_images`

This function is the primary tool for conducting image searches. It accepts several parameters to refine the search results:

- **query**: A string representing the search query or keyword.
- **limit**: An integer or float specifying the maximum number of results to return (default is 10).
- **size**: A literal value indicating the desired image size.
- **color**: A literal value for the dominant color of the images.
- **type**: A literal value specifying the type of images to search for.
- **time**: A literal value indicating the time range for the last update of images.
- **usage_rights**: A literal value for the desired usage rights of the images.
- **file_type**: A literal value specifying the image format.
- **aspect_ratio**: A literal value for the aspect ratio of the images.
- **country**: A string representing the country code for images published in a specific region.
- **safe_search**: A literal value controlling the display of explicit content.
- **region**: A string representing the country code for the region from which to make the query.
- **fields**: A string of comma-separated image fields to include in the response.

The function constructs a request to a specified endpoint, applying the provided filters, and returns the search results in JSON format. This allows users to efficiently retrieve and utilize image data tailored to their specific requirements.