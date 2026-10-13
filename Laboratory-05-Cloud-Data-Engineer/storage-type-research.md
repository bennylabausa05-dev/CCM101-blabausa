## Cloud Storage Types: Comparison

| Storage Type | Description (How does it store data?) | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| **Block Storage** | Splits data into fixed-size blocks, each with its own address. Blocks are attached to a single server as a raw volume (like a virtual hard drive), and the operating system formats it with a file system. Offers low latency and high performance. | Databases, boot volumes, and applications needing fast, low-latency random read/write access. | AWS EBS (Elastic Block Store) |
| **File Storage** | Stores data as files organized in a hierarchical directory structure (folders and subfolders), accessed over standard network protocols such as NFS or SMB. Multiple servers can mount and share the same file system at once. | Shared file systems, content management, home directories, and applications that need common access to the same files. | AWS EFS (Elastic File System) |
| **Object Storage** | Stores data as discrete objects in a flat namespace (buckets). Each object bundles the data itself, customizable metadata, and a unique identifier, and is accessed through an HTTP/REST API. Scales to virtually unlimited capacity. | Unstructured data at scale: images, videos, backups, archives, static website assets, and data lakes. | AWS S3 (Simple Storage Service) |

## Recommended for the Client

Object Storage is the best choice for your user-uploaded images because it scales automatically to hold any number of files without capacity planning, and it is far cheaper per gigabyte than block or file storage. Each image is stored with its own metadata and a unique URL-addressable key, so it can be served directly to users over HTTP and paired with a CDN for fast global delivery. It also offers very high durability (S3 is designed for 99.999999999% durability), so your users' uploads are protected against loss without extra effort on your part.

