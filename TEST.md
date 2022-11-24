# TEST CHECKLIST

## Form

### Add Group

- Add group

### Add IP Form

![Add Form](/images/add-form.png)

- Added IP address goes to the approval table
- Ping IP address:
  - If online and unregistered, IP address goes to unregistered table and cannot submit
  - If online cannot submit
- IP address referred value:
  - Start from 0(Subnet)
  - Check for gateway
  - Check for unregistered IP
  - Check for registered IP(approved/rejected)

### Edit IP Form

![Edit Form](/images/edit-form.png)

- Edited IP address goes to the approval table
- Editable field:
  - IP address
  - Group
  - Device name
  - Location
  - Description
- Ping IP address:
  - If online and unregistered, IP address goes to unregistered table and cannot submit
  - If online cannot submit

### Register User Form

![Register Form](/images/register-user.png)

- Register user:
  - If already registered, throw error

### Edit User From

![Edit User](/images/edit-user.png)

- Editable field:
  - username
  - password
  - privilege

## Table

### Inventory Table

- Edit action only for admin
- List IP Address:
  - Approved
  - Rejected

### Approval/Request Table

- List IP Address
  - Inputed
- Approve action only for admin
- Approved device/address goes to the inventory table
- Rejected device/address goes to:
  - Inventory table with red highlight
  - Rejected table

### Group Table

- Delete group also delete the IP addresses below it

### User Table

- Edit username also edit the IP address member
- Editable field:
  - username
    - if already registered, throw an error
  - privilege
  - password

## Buttons

### Export By Location

- Cannot export empty field
