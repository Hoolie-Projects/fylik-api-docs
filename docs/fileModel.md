# File model

This is file object description (model):

```typescript
interface File {
  _id: string, // File unqual ID
  name: string, // File regular name
  size: number, // File size in bytes
  type: string, // File MIME type
  expiresIn: Date, // Timestamp when file will be deleted
  createdAt: Date // Timestamp when file was uploaded
}
```
