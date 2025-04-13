

# TODO - Task-Based Freelancing Service

## **Classes to Implement:**

### 1. **User**
- Fields:
  - `id`, `name`, `email`, `password`, `dateOfJoining`
  - `List<Address> addresses`, `List<Task> currentPendingTasks`, `List<TaskOrder> pastTasks`
- Methods:
  - `register()`, `login()`, `updateProfile()`

### 2. **Address**
- Fields:
  - `id`, `apartmentDetails`, `city`, `state`, `pincode`, `addressType`, `isDefault`
- Enum: `AddressType` 
  - Values: `Home`, `Default`, `Other`

### 3. **Task**
- Fields:
  - `taskId`, `TaskType taskType`, `Freelancer assignedTo`, `User assignedFrom`, `Order orderDetails`, `TimeFrame timeDetails`
- Enum: `TaskType`
  - Values: `PLUMBING`, `MAID_SERVICE`, `ELECTRICAL`, `CARPENTRY`, `COOKING`, `PAINTING`, `LAUNDRY`

### 4. **TimeFrame**
- Fields:
  - `startTime`, `endTime`

### 5. **Order**
- Fields:
  - `orderId`, `PaymentStatus paymentStatus`, `PaymentType paymentType`, `paymentCreatedAt`

### 6. **Freelancer**
- Fields:
  - `id`, `name`, `email`, `password`, `dateOfJoining`
  - `List<Review> reviews`, `double averageRating`, `List<TaskType> tasksGoodAt`, `List<Task> assignedTasks`

### 7. **Review**
- Fields:
  - `Task task`, `String userReview`, `int rating`

### 8. **PaymentStatus** (Enum)
- Values: 
  - `PENDING`, `COMPLETED`, `FAILED`, `CANCELLED`

### 9. **PaymentType** (Interface or Enum)
- Types: 
  - `Debit/Credit`, `UPI`, `COD`

