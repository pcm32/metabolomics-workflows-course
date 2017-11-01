# Building a workflow with the fluxomics tools

You should be logged in into an instance where you had previously uploaded the sample data.

To start, we will create a new empty workflow. Do this by going to the blue menu bar on the top and press on `Workflows`.

![](images_workflows/workflows-button.png)

On the next screen press `Create new workflow`, on the right side of the screen.

![](images_workflows/create-workflows-button.png)

Name the workflow `my-fluxomics` and press `Create`

![](images_workflows/name-workflow.png)

You should now be on the workflow canvas window. Now we will select the different tools and add them to the canvas.

Click on `Fluxomics` under PHENOMENAL H2020 TOOLS and then click on `ramid` and `midcor`. You should see boxes appearing on the workflow canvas in the middle. Drag and drop the boxes so that they don't overlap, leaving `midcor` after `ramid`.

![](images_workflows/midcor-ramid.png) 

As you might remember, we run `ramid` and `midcor` separately before, and we fed the output of `ramid` into `midcor`. We will now mimick this by connecting the only output of `ramid` to `midcor`. Drag the circle with a triangle to the right of the ramid output (`outputExchange`) into the same icon available to the left of the only input of `midcor`. It should look like:

![](images_workflows/midcor-ramid-connected.png)

Now, again under Fluxomics, click on `iso2flux`, to see that box appear on the canvas. Connect the only output of `midcor` to `iso2flux` input named `tracing_data`. It should look like this:

![](images_workflows/midcor-ramid-iso2flux-connected.png)

Now your workflow is ready for running, but you need to save it first. Go to the cog icon to the upper right of the window, click on it and select `Save`.

![](images_workflows/cog-save.png)

To run it with data, press the cog icon again and select `Run` this time.

![](images_workflows/cog-run.png)

Now we need to pair the different input data files in our history to the workflow inputs. The final result with all assignments should look like this:

![](images_workflows/inputs-my-fluxomics.png)

**Please make sure that all your inputs are paired to the workflow inputs as shown, otherwise the execution will fail.** 
