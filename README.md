# Striger
## What is Striger?
Striger is an organizational format for project creation maping, and also doubles as a syntax to be parsed by the Striger Parser which creates UI blocks that elegantly display the contained project map

## How does Striger work?
Striger uses groups, keywords, and importance symbols to establish organization. Here is an example:

```
{
  outline-title: Asynk Project Manager
  features:
    –: Create/Delete Projects
    –: Assign Projects To Teams
    –: Create New Teams
    –: Assign Employees and Managers to Teams
    –: Allow client to view estimated progress
    –: Allow client access to development tests/examples
    -: Allow client to see git commits
  user-story: <Chief Operating Officer | Administrator> {
    -: Create new Teams
    -: Create/Delete Projects
    -: Assign projects to teams
    -: Assign team managers
    -: Respond to comments
  }
  user-stories: [
    user-story: <Project Manager> {
      -: Assign employees to team
      -: Update progress for client
      -: Upload releases for client
      -: Update update list for client
      -: Respond to comments
    }
    user-story: <Team Member | Employee> {
      -: View project details
      -: Respond to comments
    }
    user-story: <Client> {
      -: Write comments on updates
      -: View progress bar
      -: View Project Manager details
    }
  ]
  sprints: [
    sprint: <Sprint 1> {
      ~>: Google sign-in delegation
      -: Managers/Administrators can view projects
      ~: Administrators can create/delete Projects
      <-: Employees can view project details
    }
    sprint: <Sprint 2> {
      ~>: Admin can create new/delete teams
      -: Manager/Admin can assign team members
      -: Admin can assign managers
      <-: Client can view progress bar
    }
    sprint: <Sprint 3> {
      ~>: Manager can update progress bar
      ~: Manager can update updates
      -: Client can comment on updates
      <-: Employees can comment/leave notes on updates
    }
    sprint: <Sprint 4> {
    }
  ]
}

```

Above, you will notice that there are different 'sections' that highly resemble JSON syntax, and you wouldn't be entirely wrong. Striger is based on JSON syntax to allow for easy comprehension, and to provide a sense of familiarity. Striger's syntax reuires you to group objects in patterns which not only highly optimizes the system, but gives it a modern feel new languages like Striger need to thrive.

# Syntax
To learn about syntax, please visit the wiki section: https://github.com/kwright02/Striger/wiki

