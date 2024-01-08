# commentbox
import React, { useState } from 'react'

function Commentbox() {

    const [comment, setcomment] = useState("   ")


    const openTextbox=()=>{
        
    }
    const removeContent=()=>{
        //let newComment = " " 
        setcomment(newComment)
    }
    const handleOnChange=(event)=>{
        setcomment(event.target.value)
    }
  return (
    <>
    <div>
    <h1>{props.name}</h1>
      <div className="mb-10">
          <textarea className="form-control" id="text" rows="6" value={comment} onChange={handleOnChange}></textarea>
      </div>
      <button className="btn btn-primary mx-5" onClick={openTextbox}>Reply</button>
      <button className="btn btn-primary mx-5" onClick={removeContent} >Delete</button>
    </div>
    {/* <div>
        <h4>Preview</h4>
        <p>{comment}</p>
    </div> */}
    </>
  )
}

export default Commentbox
