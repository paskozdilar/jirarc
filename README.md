# jirarc
Bash utility for prefixing git commits with Jira Ticket ID.

## Installation
Copy `jirarc` file to a location (e.g. `~/.jirarc`) and source it in your
`~/.bashrc` (e.g. `. ~/.jirarc`).

Or just copy paste the following commands in your terminal:

    git clone https://github.com/paskozdilar/jirarc.git && \
    cp jirarc/jirarc ~/.jirarc && \
    echo >> ~/.bashrc && \
    echo '# Execute jirarc source:' >> ~/.bashrc && \
    echo '. ~/.jirarc' >> ~/.bashrc && \
    rm -rf jirarc

## Usage:
To activate, use the following command (substitute `TICKET` with Ticket ID):

    jira activate TICKET

After Ticket ID is activated, every git commit will be automatically prefixed
with `[TICKET]`.

To deactivate, use:

    jira deactivate
