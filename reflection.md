# Mission Reflection

This laboratory helped me understand object storage better because I was able to actually deploy and use one instead of just reading about it. For me, object storage is better suited for storing millions of photos because photos are unstructured data and can be stored as individual objects. If I were building a photo-sharing application, having a bucket where the photos can be organized would be more practical than treating all the photos like data on a normal computer hard drive.

Docker also made the deployment easier for me. Instead of installing MinIO manually and configuring many things separately, I was able to use one Docker command to create the MinIO container. The command also allowed me to set the username, password, and ports. At first, I was not completely familiar with all the options in the command, but after checking each part, I understood what they were doing.

I learned that a bucket is like a container for objects in object storage. In this activity, I created a bucket named `client-photos` and uploaded a sample file into it. Seeing the uploaded file inside the MinIO console helped me understand the concept better because I could actually see how an object storage system works.

For large companies, I think protecting data from physical server failures requires having more than one copy of important data. They can use backups, replication, and redundant storage in different systems or locations. This means that if one physical server fails, another copy can still be available.

My confidence in using the Linux command line is also improving. In previous activities, I was still getting used to Docker commands and Linux commands. In this activity, using commands such as `docker run` and `docker ps` felt more familiar. I realized that I do not need to memorize every command immediately; understanding what each part does is more important. Overall, this activity gave me more confidence in working with Docker, Linux, and cloud storage.

