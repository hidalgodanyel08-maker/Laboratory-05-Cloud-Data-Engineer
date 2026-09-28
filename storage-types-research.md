# Storage Types Research

## Comparison of Cloud Storage Types

| Storage Type       | Description                                                                                                                          | Primary Use Case                                                                                    | Cloud Provider Example |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------- | ---------------------- |
| **Block Storage**  | Stores data in separate blocks. It works much like a hard drive that can be attached to a computer or virtual machine.               | It is useful for operating systems, databases, and applications that need fast data access.         | AWS EBS                |
| **File Storage**   | Stores data as files inside folders and directories. Different computers or users can access the same files through a network.       | It is commonly used for shared documents, files, and folders.                                       | AWS EFS                |
| **Object Storage** | Stores data as individual objects together with information or metadata about each object. The objects are organized inside buckets. | It is useful for large amounts of unstructured data such as photos, videos, documents, and backups. | AWS S3                 |

## My Understanding

Based on my research, I think the three storage types are different mainly because of how they organize and access data. Block Storage is similar to a normal hard drive, File Storage focuses on files and folders, while Object Storage organizes data as objects inside buckets.

For the client's photo-sharing application, I think **Object Storage is the most suitable choice** because the application may need to store millions of photos. Photos are unstructured data, and object storage is designed to handle this type of data while making it easier to organize and access as the amount of stored data increases.

## My Takeaway

Before doing this activity, I mostly thought of cloud storage as simply saving files online. After comparing the three types, I learned that cloud storage has different methods depending on what kind of data an application needs to store. For a photo-sharing application, I would choose object storage because photos can be stored as objects and grouped inside a bucket.

