# **CountABC.xyz API Documentation**

This markdown document provides comprehensive documentation for the CountABC.xyz API, a service that facilitates the creation of simple numeric counters, serving as an Integer as a Service (IaaS). Through this API, users can effortlessly manage counts and events in their applications. The documentation ensures clarity in understanding the functionalities and endpoints of the API.

## **Overview**

The CountABC.xyz API offers a convenient solution for tracking various events and counts in applications. Users can create counters, reset counter values, increment or decrement counters, and count events efficiently using this API.

## **Tech Stack**

- **Endpoints**: Base API path: `https://api.countabc.xyz`
- **Data Format**: JSON
- **Cross-Origin Resource Sharing (CORS)**: Supported
- **SSL**: Supported

## **Endpoints**

### **Get Value**
- **Endpoint**: `/get/:namespace?/:key`
- **Description**: Get the value of a key.
- **Example**: `GET /get/test_namespace/test_key`

### **Set Value**
- **Endpoint**: `/set/:namespace?/:key?value=:value`
- **Description**: Set the value of a key.
- **Example**: `POST /set/test_namespace/test_key?value=10`

### **Update Value**
- **Endpoint**: `/update/:namespace?/:key?amount=:amount`
- **Description**: Update a key with +/- amount.
- **Example**: `POST /update/test_namespace/test_key?amount=5`

### **Increment Counter**
- **Endpoint**: `/hit/:namespace?/:key`
- **Description**: Increment a counter by one.
- **Example**: `POST /hit/test_namespace/test_key`

### **Create Key**
- **Endpoint**: `/create`
- **Description**: Create a key.
- **Example**: `POST /create`

### **Get Key Information**
- **Endpoint**: `/info/:namespace?/:key`
- **Description**: Get information about a key.
- **Example**: `GET /info/test_namespace/test_key`

### **Get Statistics**
- **Endpoint**: `/stats`
- **Description**: Get CountABC stats.
- **Example**: `GET /stats`

## **Usage**

Users can utilize the endpoints provided by the CountABC.xyz API to perform various operations on counters. These operations include getting the value of a key, setting the value of a key, updating a key with a specified amount, incrementing a counter by one, creating a key, retrieving information about a key, and obtaining statistics about CountABC.

## **FAQ**

- **Where is the API documentation?**: You're reading it right now.
- **Is the API free?**: Yes, it's completely free.
- **Rate Limiting?**: Key retrieving and updating have no limits. Key creation is limited to 20/IP/s.
- **Can I delete a key?**: You can't. Keys expire eventually.

## **Contact and Issues**

For any issues, suggestions, or inquiries, users can contact the CountABC.xyz team via email at [your_email@example.com](mailto:your_email@example.com).







