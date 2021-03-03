# Hierarchical list

## Required technologies (required)

- Typescript
- React
- Apollo Client

## Recommended Technologies (Optional)

- Create React App / Next.js, ....
- GraphQL Code Generator
- Router
- UI Framework (any library) or Styled Components
  - React Atlantic (@atlasgroupcz)
  - Material UI
  - React Bootstrap
  - Ant Design
- Testing
  - It is
  - React Testing Library

### Of course, you can also use other technologies to help you develop the application.

### We will be interested in technologies you used (or didn't use)

## Task

The **GraphQL** server is running at url https://react-test.atlasconsulting.cz/. ([Server provides playground](https://react-test.atlasconsulting.cz/)).
Your task is to create an application that will communicate with this server.
The application will be able to draw a hierarchical structure (folder / file) when clicking on an item
file, a preview is displayed.
The server contains two queries.

**1. query** returns a list of items that the application will use to list the hierarchical list.
(The item has information about whether to behave as a folder or as a file)
The input parameter is the id of the folder, if the parameter is empty, the API returns the first level (root folder),
the output is then a list of items that belong to this folder.

**2. query** returns the data of the given file, the input parameter is id.

###You will submit a **GIT** repository with the application source files.

## Bonus
- close the preview
- expand and collapse components
- cache of hierarchical structure
- cache of open files
- history of open files
- bookmarks with files
  - the user can open files from a hierarchical structure
  - When you open a file, a preview of the file is displayed
  - the application saves open files
  - the user has access to the list of open files ^
  - the user can close open files from the list
- application bookmarks
  - the user can dynamically create and delete independent bookmarks (as open bookmarks)
    bookmarks in the browser or desktop in the operating system)
  - each new tab will look like a new application with a basic state (with
    closed hierarchical list, no preview and no list of open files, the solution must be within one react application)

[Application Reference Design](https://wireframe.cc/6JRvnm)
