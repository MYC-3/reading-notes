# Room
[Notes taken from this site](https://developer.android.com/training/data-storage/room)

- Room provides the following benefits:
  - Compile-time verification of SQL queries.
  - Convenience annotations that minimize repetitive and error-prone boilerplate code.
  - Streamlined database migration paths.
- Add these dependencies to the `build.gradle` file:

```Java
dependencies {
    def room_version = "2.3.0"

    implementation "androidx.room:room-runtime:$room_version"
    annotationProcessor "androidx.room:room-compiler:$room_version"

    // optional - RxJava2 support for Room
    implementation "androidx.room:room-rxjava2:$room_version"

    // optional - RxJava3 support for Room
    implementation "androidx.room:room-rxjava3:$room_version"

    // optional - Guava support for Room, including Optional and ListenableFuture
    implementation "androidx.room:room-guava:$room_version"

    // optional - Test helpers
    testImplementation "androidx.room:room-testing:$room_version"

    // optional - Paging 3 Integration
    implementation "androidx.room:room-paging:2.4.0-beta01"
}
```
- 3 major components of Room:
 1. *Database class* that holds the database and serves as the main access point for the underlying connection to your app's persisted data.
 2. *Data entities* that represent tables in your app's database.
 3. *Data access objects (DAOs) that provide methods that your app can use to query, update, insert, and delete data in the database.

## Room Entities
[Notes taken from this site](https://developer.android.com/training/data-storage/room/defining-data)

- You define each Room entity as a class that is annotated with `@Entity`. Example:

```Java
@Entity
public class User {
    @PrimaryKey
    public int id;

    public String firstName;
    public String lastName;
}
```

## Relationships between objects
[Notes taken from this site](https://developer.android.com/training/data-storage/room/relationships)

## Accessing data using Room DAOs
[Notes taken from this site](https://developer.android.com/training/data-storage/room/accessing-data#java)

- >When you use the Room persistence library to store your app's data, you interact with the stored data by defining data access objects, or DAOs.
- >Room provides convenience annotations for defining methods that perform simple inserts, updates, and deletes without requiring you to write a SQL statement.
- Convenience methods:
  - Insert
  - Update
  - Delete
  - Query

[Back to HOME](../README.md)