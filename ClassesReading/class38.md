# Android Reading 12

## What are the three criteria an acticity’s intent filter must fulfill in order for a system to send an intent to that activity?

- Action Match: The intent filter must specify the action being requested by the sender. It indicates the type of operation to be performed. For example, an activity might specify that it can handle the "VIEW" action, indicating it can display data.
- Category Match: The intent filter must specify the category or categories the activity supports. Categories represent additional information about the action or component. Common categories include "DEFAULT" for activities that are a default part of the application, and "BROWSABLE" for activities that can be invoked from a web browser.
- Data Match (Optional): The intent filter can specify data that should be present in the intent. This includes the type of data, the scheme, host, and path. For instance, an activity might specify that it can handle "http" schemes or data with a specific MIME type.

## How does an activity retrieve the Intent that it was started by?

In Android, an activity retrieves the Intent that started it by calling the getIntent() method. This method is provided by the Activity class and allows the activity to access the Intent object containing the information passed to it during its launch. The retrieved Intent can then be used to extract various data, such as extras or parameters, that was included when the activity was started. This mechanism is commonly used to pass information between different activities within an application, allowing them to communicate and share data. The getIntent() method is typically called in the onCreate() method or other relevant lifecycle methods of the activity to access the Intent at the time of its creation.

## Explain intents to a non-technical friend

Imagine Intents in Android as messengers that help different parts of your phone communicate with each other. Let's say you're using an app and decide to share a photo. When you tap the share button, the app creates an "Intent," a kind of virtual envelope containing instructions like "share this image." The Intent is then passed to the system, which figures out the best way to handle it—maybe opening a list of messaging apps. Intents help apps send messages and instructions to each other, making your phone's features work seamlessly together, whether it's sharing a photo, opening a link, or starting a new activity. So, in simple terms, Intents make your phone apps talk to each other to get things done.

## Compare and contrast implicit and explicit intents

Implicit and explicit intents are two types of communication mechanisms in Android. Explicit intents are like a direct address on an envelope; you know exactly where it's going. In Android, you explicitly mention the target component (activity or service) by its name or class when creating an explicit intent. It's great for situations when you know exactly what component you want to start.

## What is the primary information contained within an Intent?

An Intent in Android primarily contains information about an operation to be performed, serving as a message that can trigger activities, services, or broadcast receivers. It includes details such as the action to be performed (like opening a webpage or sending a message), the data associated with the action (like a URI or content), the target component (in explicit intents), and additional parameters or metadata. Intents facilitate communication between different components of an Android application or even between different applications, allowing them to request functionality or share information seamlessly.
