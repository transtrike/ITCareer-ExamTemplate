# ITCareer-ExamTemplate
'Cuz why not

## For Migrations:

I. ADD CONNECTION STRING AND EDIT DATABASE(`app.UseNpgsql()` to `app.UseMySql()` or whatever)!!!

II. Open CMD/Powershell

III. Navigate to the `Project.Data Folder`
- `cd Data/Project.Data`

IV. Run migrations command(Use StartUpProject flag, because the project does not have a DbContextFactory!):
- `dotnet ef migrations add Initial -s ../../Project.Web`

OR

- `Add-Migration InitialCreate -StartUpProjectName ../../Project.Web`

You don't even need to apply the migrations, since they get seeded at application startup
