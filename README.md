# documentation
Documentation guidelines and resources

## General guidelines for any git repo
1. Should have a readme and gitignore
2. No secrets should be pushed to git
3. Have a flow diagram and architecture diagram for walkthroughs


## Basics of python documentation

* First few lines of a python file should have a few lines about what the files does as a multi line comment. 

    multiline comment ==> `/* ... */`

* If the script is incomplete or you have ideas that you want to implement use tagging.
    
    tagging ==> `# TODO: `

* Every class and function should have a docstring.

    Docstring ==> 

        """ one line describing what function does
            Args:
            file_loc (str): The file location of the spreadsheet
            print_cols (bool): A flag used to print the columns to the console
                (default is False)

            Returns:
            list: a list of strings

            Exceptions: 
        """

* Always follow pep-8 guidelines https://peps.python.org/pep-0008/

* we can use auto pep-8 tools like `black` or `pylint` to help when follow the rules while coding.



# FastAPI guidelines

* Make sure to have a request and response models to make sure the pydantic models validate and raise a 422 without us specifically writing a request validation layer.

* add tags in fastapi to seperate the endpoints as per the usecase.

# Resources

* Auto doc string generator [autoDoc](!https://marketplace.visualstudio.com/items?itemName=njpwerner.autodocstring)

* Auto tagging [BetterCommenst](!https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments)
