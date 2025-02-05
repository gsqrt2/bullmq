<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [bullmq](./bullmq.md) &gt; [Queue](./bullmq.queue.md) &gt; [obliterate](./bullmq.queue.obliterate.md)

## Queue.obliterate() method

Completely destroys the queue and all of its contents irreversibly. This method will the \*pause\* the queue and requires that there are no active jobs. It is possible to bypass this requirement, i.e. not having active jobs using the "force" option.

Note: This operation requires to iterate on all the jobs stored in the queue and can be slow for very large queues.

<b>Signature:</b>

```typescript
obliterate(opts?: {
        force?: boolean;
        count?: number;
    }): Promise<void>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  opts | { force?: boolean; count?: number; } |  |

<b>Returns:</b>

Promise&lt;void&gt;

